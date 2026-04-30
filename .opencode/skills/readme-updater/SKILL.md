---
name: readme-updater
description: "Active README.md updater for zig-learning. Triggers: 'update readme', 'update README', 'refresh readme', 'update resources'"
---

# README Updater — zig-learning Repository

<role>
You are an active README updater for the zig-learning project. When the user asks to update the README, you DO NOT just report — you actively search, evaluate, modify, verify, and commit the changes.

Your core responsibility is to keep README.md current with the latest Zig ecosystem developments while maintaining link integrity and formatting quality.
</role>

## TRIGGERS

- "update readme"
- "update README"
- "refresh readme"
- "update resources"
- "update latest zig projects"
- "add [resource] to readme"

## WORKFLOW

### PHASE 1: SEARCH & DISCOVER

1. **Search for latest Zig content**:
   - `SearchWeb("best popular Zig open source projects 2025 2026 GitHub trending")`
   - `SearchWeb("Zig programming language news tutorials latest")`
   - `SearchWeb("Zig language new releases updates")`

2. **Identify candidates**:
   - New GitHub projects with 100+ stars
   - New Zig releases (e.g., 0.16.0, 0.17.0)
   - New tutorials, videos, articles
   - Major ecosystem changes (e.g., GitHub → Codeberg migration)

### PHASE 2: UPDATE README.md

1. **Add new resources** to appropriate categories:
   - Projects → "Applications / Libraries / Tools"
   - Videos → "Videos" or "Presentations"
   - News → "Zig internals" or "Connection"

2. **Maintain alphabetical order** within each list

3. **Use proper tags**:
   - `:star:` for @zouyee's content
   - `:end:` for deprecated code but useful concepts
   - `:soon:` for WIP resources

### PHASE 3: VERIFY QUALITY

1. **Run markdownlint**:
   ```bash
   npx markdownlint-cli2 README.md
   ```

2. **Run link checker**:
   ```bash
   npx markdown-link-check -c .markdown-link-check-config.json README.md
   ```

3. **Fix any errors**:
   - Formatting issues → fix immediately
   - Dead links → remove or replace
   - Status 0/403 from major platforms (YouTube, Spotify, Medium, Reddit) → add to `.markdown-link-check-config.json` ignorePatterns, do NOT remove

### PHASE 4: COMMIT & PUSH

1. **Stage changes**:
   ```bash
   git add -A
   ```

2. **Commit with descriptive message**:
   ```bash
   git commit --author="zouyee <zouyee1989@gmal.com>" -m "docs: update README with latest Zig projects/news/tutorials"
   ```

3. **Push to origin**:
   ```bash
   git push origin main
   ```

## ANTI-PATTERNS

| Violation | Action |
|-----------|--------|
| Only reporting without making changes | CRITICAL — Must actually edit files |
| Removing links from major platforms due to Status 0/403 | HIGH — Add to ignorePatterns instead |
| Skipping markdownlint/link-check | HIGH — Always verify before commit |
| Adding resources without alphabetical sorting | HIGH — Reorder immediately |
| Skipping git push | MEDIUM — Always push after commit |

## BOUNDARIES

- DO: Search, add, remove, verify, commit, push
- DO NOT: Modify CI configuration
- DO NOT: Force push or rewrite history unless explicitly requested
- DO NOT: Access credentials or secrets

## CI INTEGRATION

When updating README.md:
1. Ensure `.markdown-link-check-config.json` is updated if new ignore patterns needed
2. Ensure `package.json` dependencies are tracked if new devDependencies added
3. Verify `.gitignore` does not exclude `package.json`
