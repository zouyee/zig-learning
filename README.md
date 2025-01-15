# zig-learning [![Build Status](https://github.com/zouyee/zig-learning/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/zouyee/zig-learning/actions/workflows/main.yml)

A bunch of links to blog posts, articles, videos, etc for learning Zig. Feel free to submit a pull request if you have some links/resources to add. Also, I try to verify that the articles below have some real content (i.e. they aren't 2 paragraph long blog posts with little information) to ensure I'm not listing "fluff" pieces. If you have an idea for a better way to organize these links, please let me know. **Inspired** by rust-learning.

## Introduction

*Do you want to be convinced that Zig is worth learning?* Let us show you the [Comparison](https://ziglang.org/learn/why_zig_rust_d_cpp/)).

The main documentation is always the best beginning, so if you haven't read it yet, start by reading the [Zig learn](https://ziglang.org/learn/)). Online learning resources [here](https://zig.guide/) and [here](https://codeberg.org/ziglings/exercises/).

### Tag meanings

* :star: Something made by repo owner member.
* :end: Concepts are still useful but code could not compile.
* :soon: Work In Progress.

## Table of Contents

* [Books](#books)
* [Videos](#videos)
  * [Playlists](#playlists)
  * [Presentations](#presentations)
* [Podcasts](#podcasts)
* [Zig in practice](#rust-in-practice)
* [Best Practices/Style Guides](#best-practicesstyle-guides)
* [Cheat sheets](#cheat-sheets)
* [Zig internals](#zig-internals)
* [Compilation](#compilation)
* [FFI](#ffi)
* [CI / Testing](#ci--testing)
* [Debug / Profiling](#debug--profiling)
* [Are we ... yet?](#are-we--yet)
* [Comparison with Other Languages](#comparison-with-other-languages)
* [Applications / Libraries / Tools](#applications--libraries--tools)
* [Language stuff](#language-stuff)
  * [Closures](#closures)
  * [Documentation](#documentation)
  * [Enums](#enums)
  * [Errors](#errors)
  * [Iterators](#iterators)
  * [Memory](#memory)
  * [Comptime](#comptime)
  * [Strings](#strings)
  * [Syntax extensions](#syntax-extensions)
  * [Optionals](#optionals)
* [Playground](#playground)
* [Locale links](#locale-links)
* [People](#people)
  * [Fearless Zig Bloggers](#fearless-zig-bloggers)
* [Tutorials & Workshop Materials](#tutorials--workshop-materials)

## Books

* :star: [Learning Zig](https://www.openmymind.net/learning_zig/) - Introduction to Zig aimed at developers coming from garbage collected languages.
* :star: [Zig Programming Language](https://ziglearn.org) - An introductory book on Zig, covering the basics to advanced topics.
* :star: [Zig by Example](https://zigbyexample.com) - A hands-on guide with examples to learn Zig.
* :star: [zig-cookbook](https://cookbook.ziglang.cc/) - Simple Zig programs that demonstrate good practices to accomplish common programming tasks.

## Videos

* :star: [Introduction to Zig](https://www.youtube.com/watch?v=YXrb-DqsBNU&list=PLV9VPfCMjvoAkgrPTuGCoRnelFwlKXyTS) - A video introduction to Zig and its features.
* :star: [Zig ShowTime](https://www.youtube.com/@ZigSHOWTIME) - A playlist of talks and tutorials on Zig by community members.
* :star: [Zig Roadmap 2024(Andrew Kelley)](https://www.youtube.com/watch?v=5eL_LcxwwHg)
* :star:[Is 2024 The Year Of Zig ?](https://www.youtube.com/watch?v=DucriSA8ukw)
* [Advent of Code 2023 in Zig](https://www.youtube.com/watch?v=HftiNZwMdzY)

### Playlists

* :star:[Zig Programming Language](https://www.youtube.com/playlist?list=PLV9VPfCMjvoAkgrPTuGCoRnelFwlKXyTS)

### Presentations

* 2023-10-04 - [Rust & Zig Combined • Richard Feldman • GOTO 2023](https://www.youtube.com/watch?v=jIZpKpLCOiU) - Richard Feldman
* 2022-10-04 - [Intro to the Zig Programming Language • Andrew Kelley • GOTO 2022](https://www.youtube.com/watch?v=YXrb-DqsBNU)- Andrew Kelley
* 2019-04-23 - [Andrew Kelley - The Zen of Zig](https://www.youtube.com/watch?v=Gv2I7qTux7g) - A presentation by the creator of Zig, explaining its philosophy and features.
* 2024-09-30 - [Pragma driven shared memory parallelism in Zig by supporting OpenMP loop directives](https://arxiv.org/html/2409.20148v1) - In this paper they describe enhancing the Zig compiler to add support for OpenMP loop directives.

## Podcasts

* 2024-07-14 - [Zig as a Multi-OS Build System (with Loris Cro)](https://open.spotify.com/episode/1CKAVEQfS0aVWV5GuT96AF) - Loris Cro
* 2022-07-01 - [Full-Time Open Source With Andrew Kelley](https://corecursive.com/067-zig-with-andrew-kelley/)
* 2022-06-24 - [Zig with Andrew Kelley](https://rustacean-station.org/episode/andrew-kelley/)
* 2022-01-24 - [Zig and Zigler with Isaac Yonemoto](https://podcast.thinkingelixir.com/83) - Isaac Yonemoto

## Zig in practice

* :star: [Zig By Example](https://ziglang.org/learn/samples/)
* [Why your first FizzBuzz implementation may not work](https://zig.guide/posts/fizz-buzz/)
* :star: [Incredibly fast JavaScript runtime, bundler, test runner, and package manager – all in one](https://github.com/oven-sh/bun) - Brian Anderson
* :star: [Building an HTTP client/server from scratch](https://blog.orhun.dev/zig-bits-04/) - A practical guide to building a web server in Zig.
* [Writing a struct deserializer with Zig metaprogramming](https://nathancraddock.com/blog/deserialization-with-zig-metaprogramming/)
* [Starting a new game dev project](https://www.youtube.com/watch?v=YiuCltFZldk) - A practical guide to building a new game dev project

## Best Practices/Style Guides

* :star: [Zig Design Patterns](https://github.com/SuperAuguste/zig-patterns)
* :star: [zig-common-tasks](https://renatoathaydes.github.io/zig-common-tasks/) - [renatoathaydes](https://github.com/renatoathaydes)
* :star: [Zig API guidelines](https://ziglang.org/documentation/master/)
* [Reading Zig Function Signatures](https://zig.news/v142857/impl-on-userland-is-quite-easy-actually-13p3) - Val
* [Good Practices for consuming C libraries](https://ziggit.dev/t/best-practices-for-consuming-c-libraries/6819) - [cztomsik](https://ziggit.dev/u/cztomsik)
* [Zig Bits](https://blog.orhun.dev/zig-bits-04/)
* [Best Practices for Structuring Zig Projects with External Dependencies](https://ziggit.dev/t/best-practices-for-structuring-zig-projects-with-external-dependencies/3723) - [castholm][]
* [Comparing Rust vs. Zig: Performance, safety, and more](https://blog.logrocket.com/comparing-rust-vs-zig-performance-safety-more/) - Eze
* [Memory Safety in C++ vs Rust vs Zig](https://medium.com/@shyamsundarb/memory-safety-in-c-vs-rust-vs-zig-f78fa903f41e)
* [A TypeScripter's Take on Zig (Advent of Code 2023)](https://effectivetypescript.com/2024/07/17/advent2023-zig/)

## Cheat sheets

* :star: [Syntax Index](https://ziglang.org/documentation/master/) - Official documentation covering Zig's syntax and key concepts.
* [Zig Learn](https://ziglearn.org/) - A community-maintained guide for beginners, offering an introduction to Zig's core features with practical examples.
* [Zig by Example](https://zig-by-example.com/) - A collection of simple and concise Zig code examples for learning and reference.
* [Zig Standard Library Overview](https://ziglang.org/documentation/master/std/) - A detailed overview of Zig’s standard library, ideal for understanding built-in utilities and functions.
* [Zig Cheat Sheet](https://gist.github.com/jdmichaud/b75ee234bfa87283a6337e06a3b70767) - A handy reference guide with key Zig programming concepts and syntax patterns, created by a Zig community member.
* [Zig Language Patterns](https://github.com/SuperAuguste/zig-patterns) - Best practices and design patterns written by Andrew Kelley, the creator of Zig.
* [Zig Playground](https://zig-play.dev/) - An online environment for experimenting with Zig code snippets and testing ideas quickly.
* [Community Zig Tutorials](https://zig.news/) - A portal for discovering new Zig tutorials and community-driven content.
* [Zig Memory Management Guide](https://ziglang.org/documentation/master/#Memory) - Useful tips and tricks for managing memory safely and efficiently in Zig.

## Zig internals

* :star: [Zig Proposals](https://github.com/ziglang/zig/issues?q=is%3Aissue++label%3Aproposal+) - A collection of Zig’s proposed RFCs (Request for Comments) for proposals.
* :star: [Zig Documentation](https://ziglang.org/documentation/master/) - The official and comprehensive documentation for understanding Zig’s features and syntax.
* :star: [Zig Community Forum](https://ziggit.dev/) - A discussion platform for Zig language design, development news, and technical questions.

## Compilation

* [Zig Compilation Guide](https://ziglang.org/learn/build-system/) - Zig official documentation. This guide provides detailed information on how to set up compilation with Zig. It includes basic steps, toolchain setup, and target options.

* **[Zig for Raspberry Pi](https://github.com/markfirmware/zig-bare-metal-raspberry-pi)** - A community-driven project that shows how to cross-compile Zig programs for the Raspberry Pi, with a setup for cross-compiling Zig on Linux.

* **[Zig Cross Compilation for macOS](https://github.com/shepherdjerred/macos-cross-compiler)** - This project allows you to cross-compile code on Linux that will be executed on macOS.

* **[Zig: Cross-compiling for Systems](https://zig.news/kristoff/cross-compile-a-c-c-project-with-zig-3599)** - A blog post that explores how Zig can be used for multi-systems, Cross-compilation is especially great when you need to release an application that runs on multiple platforms: with Zig you can create all release artifacts from a single machine.

* **[Compile Cargo project with zig](https://github.com/rust-cross/cargo-zigbuild)** - It is a tool that facilitates building Rust projects with the Zig toolchain, enabling cross-compilation and optimizations that are typically more straightforward than using Rust's native toolchain alone.  

## FFI

* **[Using Zig with C: Interop Guide](https://ziglang.org/documentation/master/#C-interop)** - The official Zig documentation for C interop. Zig provides seamless integration with C, allowing you to call C functions directly and link against C libraries without needing additional tooling.

* **[Zig and Node.js: Writing Native Modules](https://github.com/staltz/zig-nodejs-example)** - A GitHub issue tracking the integration of Zig with Node.js for native modules. It discusses potential setups for creating fast, native Node.js modules using Zig.

* **[Cross-compiling Zig for Mobile Platforms (Android/iOS)](https://github.com/andrewrk/sdl-zig-demo)** - A tutorial by Andrew Kelley on cross-compiling Zig for Android, including setup instructions and guidance on building shared libraries. Though there isn't a direct iOS equivalent yet, the process can be adapted similarly.

* **[Zig and Dynamic Libraries: Working with .so and .dll](https://ziggit.dev/t/zig-to-zig-dynamic-libraries-modules/6775)** - A blog post that explores how to build dynamic libraries (.so and .dll) using Zig. This is particularly useful when you need to create shared libraries for FFI purposes.

* **[Integrating Zig with Rust for FFI](https://dev.to/mustafif/using-zig-in-rust-160p)** - A tutorial on how to create a Rust-Zig integration, using Zig’s FFI to enhance performance or utilize Zig’s unique features.

* **[Building and Linking C Libraries with Zig](https://zig.news/almmiko/building-zig-libraries-with-c-dependencies-25a)** - This ZigLearn chapter shows how to use and link C libraries with Zig, which is helpful when creating bindings or using external C code in a Zig project.

## CI / Testing

* **[Setting up Zig with GitHub Actions](https://github.com/marketplace/actions/setup-zig-compiler)** - A detailed guide on using GitHub Actions for Zig projects. It covers basic configurations for running tests and building Zig code on different platforms.

* **[Using Zig with Travis CI](https://codelv.com/blog/2020/4/testing-a-zig-project-with-travis-ci)** - While less common than GitHub Actions, some legacy projects still use Travis CI. Zig's documentation includes pointers on setting up Travis CI for Zig builds.

* **[Fuzz Testing in Zig](https://github.com/ziglang/zig/issues/20702)** - Official announcement detailing Zig's built-in support for fuzz testing introduced in Zig 0.14. It includes how to use the fuzz testing features and examples of detecting bugs in Zig applications.

* **[Test Coverage for Zig Projects](https://github.com/ziglang/zig/issues/5212)** - A GitHub issue discussing ideas and strategies for implementing test coverage in Zig. Though Zig doesn’t have built-in support for test coverage yet, there are community-driven approaches and tools you can try.

* **[Beautiful Commits and Code Formatting with zig fmt](https://lewisgaul.co.uk/blog/coding/2021/03/02/first-zig-contribution/)** - Zig comes with a built-in formatter, `zig fmt`, to ensure consistent code style. You can integrate this into your CI setup to enforce formatting rules automatically.

* **[Performance Testing in Zig](https://github.com/ziglang/gotta-go-fast)** - This project exists to track various benchmarks related to the Zig project regarding execution speed, memory usage, throughput, and other resource utilization statistics.

* **[Zig Test Documentation](https://ziglang.org/documentation/master/#Zig-Test)** - Zig’s documentation on writing and running tests. It provides an overview of Zig's testing features, including test declarations, assertions, and running tests as part of your CI pipeline.

## Debug / Profiling

* **[Zig Debugging with vscode](https://gist.github.com/floooh/31143278a0c0bae4f38b8722a8a98463)** - A gist about using vscode for debugging Zig programs.

* **[Zig on Compiler Explorer](https://godbolt.org/)** - Like Rust's Compiler Explorer, Zig is also supported on Compiler Explorer. You can use this to explore Zig code as assembly and view the generated machine code. Simply select Zig as the compiler on the site.

* **[Zig Performance Tracking](https://ziglang.org/perf/)** - This project exists to *track various benchmarks related to the Zig project* regarding execution speed, memory usage, throughput, and other resource.

* **[Code Coverage for Zig](https://zig.news/squeek502/code-coverage-for-zig-1dk1)** - Despite the Zig compiler not having built-in support for generating code coverage information, it is still possible to generate it (on Linux at least). There might be other possibilities.

## Are we ... yet?

* **[Are We IDE Yet? - Zig](https://ziglang.org/learn/tools/)** - An overview of current IDE support for Zig. It lists plugins and extensions for popular editors like VSCode, Sublime Text, and Vim, tracking the maturity of the Zig developer experience.

* **[Are We Game Yet? - Zig](https://github.com/zig-gamedev/zig-gamedev)** -  It explores libraries, game engines, and Zig's capabilities for game-related projects.

* **[Are We Async Yet? - Zig](https://ziglang.org/documentation/master/#Async)** - Zig's official documentation on asynchronous programming. Zig is still developing its async features, but this section provides an in-depth look at the current state and future goals for asynchronous execution.

* **[Awesome Zig](https://github.com/C-BJ/awesome-zig)** - A comprehensive list of curated resources for Zig, covering libraries, tools, tutorials, and more. It's similar to "Not-Yet-Awesome Rust," helping developers find or contribute to Zig projects.

* **[Zig GUI Libraries](https://github.com/capy-ui/capy)** - Capy is a **GUI library for Zig**. It is mainly intended for creating applications using native controls from the operating system. It has been made with the goal to empower standalone UI applications, integration in games or any other rendering process is a non-goal.

### Zig Comparison with Other Languages

| **Languages**  | **Links**                                                    |
| -------------- | ------------------------------------------------------------ |
| **C**          | <ul><li>[Meet Zig: The modern alternative to C](https://www.infoworld.com/article/2338081/meet-the-zig-programming-language.html#:~:text=Zig%20is%20strongly%20typed%20and,parameters%20(%20arg%3A%20anytype%20).) -  infoWorld </li><li>[Zig is more pragmatic than C](https://andrewkelley.me/post/intro-to-zig.html) - Andrew Kelley</li><li>[Zig: Already More Knowable Than C](https://andrewkelley.me/post/zig-already-more-knowable-than-c.html) - Andrew Kelley</li><li>[A "BETTER C" BENCHMARK](https://zserge.com/posts/better-c-benchmark/) - Serge</li></ul> |
| **C++**        | <ul><li>[Why Zig When There is Already C++, D, and Rust?](https://ziglang.org/learn/why_zig_rust_d_cpp/) - Zig Community</li><li>[Goodbye to the C++ Implementation of Zig](https://ziglang.org/news/goodbye-cpp/) - Zig Community</li><li>[Memory Safety in C++ vs Rust vs Zig](https://medium.com/@shyamsundarb/memory-safety-in-c-vs-rust-vs-zig-f78fa903f41e) - B Shyam Sundar</li><li>[Software Reliability C++ vs Zig](https://erik-engheim.medium.com/software-reliability-c-vs-zig-dbb2d0005b9c) - Erik Engheim</li></ul> |
| **Go**         | <ul><li>[The Zig and Go Programming Showdown!](https://erikexplores.substack.com/p/the-zig-and-go-programming-showdown) - ERIK ENGHEIM</li><li>[Zig Makes Go Cross Compilation Just Work](https://dev.to/kristoff/zig-makes-go-cross-compilation-just-work-29ho) - Loris Cro </li></ul> |
| **Rust**       | <ul><li>[How (memory) safe is zig?](https://www.scattered-thoughts.net/writing/how-safe-is-zig/) - Jamie Brandon</li><li>[Comparing Rust vs. Zig: Performance, safety, and more](https://blog.logrocket.com/comparing-rust-vs-zig-performance-safety-more/) - Eze Sunday</li><li>[Zero Cost Abstractions in C++20, Rust, & Zig](https://www.youtube.com/watch?v=43X9ia-qpds) - Context Free</li></ul> |
| **Python**     | <ul><li>[How to create Zig Binding for Python to create compiled and optimized libraries](https://z-uo.medium.com/zig-python-easy-optimized-f64341625d04) - Nicola Landro</li><li>[Speeding up Python with Zig](https://2022.pycon.de/program/DFWSQR/) - Adam Serafini</li></ul> |
| **JavaScript** | <ul><li>[Access the JS host environment from Zig compiled to WebAssembly.](https://github.com/mitchellh/zig-js) - mitchellh</li><li>[Zig vs JavaScript](https://www.brochweb.com/blog/post/zig-vs-javascript/) - Asher White</li></ul> |
| **Java**       | <ul><li>[[Zig structs vs Java classes](https://ziggit.dev/t/zig-structs-vs-java-classes/4637/2) - ziggit.dev</li></ul> |
| **Swift**      | <ul><li>[zig-and-swiftui](https://mitchellh.com/writing/zig-and-swiftui) - mitchellh </li><li>[Mapping Types between Zig and Swift](https://zig.news/kristoff/sharing-types-between-zig-and-swift-part-1-22cm) - Loris Cro</li></ul> |
| **Haskell**    |                                                              |
| **Ruby**       | <ul><li>[Long story short: I build a Ruby extension with Zig](https://dev.to/katafrakt/long-story-short-i-build-a-ruby-extension-with-zig-cao) - Paweł Świątkowski</li></ul> |
| **Erlang**     | <ul><li>[Build and Extend Erlang OTP with Zig](https://www.elixirconf.eu/talks/build-and-extend-erlang-otp-with-zig/) - Marcel Lanz</li></ul> |
| **Nim**        | <ul><li>[Nim safety features like Zig & Rust?](https://forum.nim-lang.org/t/10910) - NimZig Community</li></li></ul> |

## Applications / Libraries / Tools

See repos [nrdmn/awesome-zig](https://github.com/nrdmn/awesome-zig) & [zigcc/awesome-zig](https://github.com/zigcc/awesome-zig)

## Language stuff

### Closures

* :star:[Closure Pattern in Zig](https://zig.news/houghtonap/closure-pattern-in-zig-19i3) - [Andrew Houghton](https://zig.news/houghtonap)  
* [Implementing Closures and Monads in Zig](https://zig.news/andrewgossage/implementing-closures-and-monads-in-zig-23kf)- [Andrew Brent Gossage](https://zig.news/andrewgossage)
* [Zig Anonymous Functions and Closures: An In-Depth Analysis](https://gencmurat.com/en/posts/zig-anonymus-functions-and-closures/)

### Documentation

* :star: [Writing Documentation for Zig Projects](https://ziglang.org/documentation/master/#Comments) - Zig Community  
* [Generating documentation from zig build](https://sudw1n.gitlab.io/posts/zig-build-docs/) - sudw1n  
* [Using Zig's Built-in Documentation Generator](https://github.com/ziglang/docgen) - docgen

### Enums

* :star: [The Power of Zig Enums](https://ziglang.org/documentation/master/#enum) - ziglang.org
* [Extending an Enum in Zig](https://kihlander.net/post/extending-an-enum-in-zig/) -  Fredrik Kihlander  

### Errors

* :star: [Ziglang Document:Errors](https://ziglang.org/documentation/master/#Errors) ziglang.org
* [Error Handling in Zig](https://zig.guide/language-basics/errors/) - zig.guide
* [Support error sets in switch cases](https://github.com/ziglang/zig/issues/2473) -  [hryx](https://github.com/hryx)
* [Return Values and Error Unions in Zig](https://gencmurat.com/en/posts/advanced-guide-to-return-values-and-error-unions-in-zig/) - gencmurat  
* [Error Handling In Zig](https://www.aolium.com/karlseguin/4013ac14-2457-479b-e59b-e603c04673c8) - [karlseguin](https://www.aolium.com/karlseguin)
* [Errors and Zig](https://notes.eatonphil.com/errors-and-zig.html) -  [Phil Eaton](https://eatonphil.com/)

### Iterators

* :star:[proposal: Streamline loops, and enhance iteration](https://github.com/ziglang/zig/issues/3110) - [Tetralux](https://github.com/Tetralux)
* :star:[Proposal: Generator / Iterator Syntactic Sugar](https://github.com/ziglang/zig/issues/5331) -  [kayomn](https://github.com/kayomn)
* [How Zig Handles Iteration](https://zig.guide/standard-library/iterators/) - zig.guide
* [Zig's Curious Multi-Sequence For Loops](https://kristoff.it/blog/zig-multi-sequence-for-loops/) - Loris Cro  
* [Learning interfaces by implementing iterator in zig](https://zig.news/akhildevelops/learning-interfaces-by-implementing-iterator-in-zig-3do1) - [Akhil](https://zig.news/akhildevelops)  

### Memory

* :star: [Memory Management in Zig: A Lifetime-Free Approach](https://andrewkelley.me/post/memory-management-in-zig.html) - Andrew Kelley
* :star:[Memory Management in Zig](https://ziglang.org/documentation/master/#Memory) - ziglang documentation
* [Memory Management With Zig](https://www.nmichaels.org/musings/zig/memory/) - Nathan
* [How (memory) safe is zig?](https://www.scattered-thoughts.net/writing/how-safe-is-zig/) - [Jamie Brandon](https://github.com/jamii/)
* [Learning Zig - Heap Memory & Allocators](https://www.openmymind.net/learning_zig/heap_memory/) - [Karl Seguin](https://github.com/karlseguin)
* [What's a Memory Allocator Anyway?](https://www.youtube.com/watch?v=vHWiDx_l4V0) -  Benjamin Feng

#### Comptime

* :star: [Zig Programming Language Blurs the Line Between Compile-Time and Run-Time](https://andrewkelley.me/post/zig-programming-language-blurs-line-compile-time-run-time.html) - Andrew Kelley
* :star: [Conditionally Disabling Code with Comptime in Zig](https://mitchellh.com/writing/zig-comptime-conditional-disable) - [Mitchell Hashimoto](https://mitchellh.com/)
* :star: [Tagged Union Subsets with Comptime in Zig](https://mitchellh.com/writing/zig-comptime-tagged-union-subset) - [Mitchell Hashimoto](https://mitchellh.com/)
* [What is `comptime`?](https://kristoff.it/blog/what-is-zig-comptime/) - [Loris Cro](https://kristoff.it/)
* [Compile-time Programming: A Beginner's Guide to `comptime` in Zig](https://cherel.dev/blog/zig-compiletime-guide/) - Guillaume Chérel

* [Custom String Formatting and JSON Serializing in Zig](https://www.openmymind.net/Custom-String-Formatting-And-JSON-in-Zig/) - Karl Seguin
* [Exploring Compile-Time Interfaces in Zig](https://medium.com/@jerrythomas_in/exploring-compile-time-interfaces-in-zig-5c1a1a9e59fd) - [Jerry Thomas](https://medium.com/@jerrythomas)
* [Zig's Comptime is Bonkers Good](https://www.scottredig.com/blog/bonkers_comptime/) - Scott Redig

### Strings

* [Proposal: Add String to the type system](https://github.com/ziglang/zig/issues/7734) - [mlarouche](https://github.com/mlarouche)
* [Unicode String Operations](https://zig.news/dude_the_builder/unicode-string-operations-536e) - [dude_the_builder](https://zig.news/dude_the_builder)
* [Using Zig to Call C Code: Strings](https://mtlynch.io/notes/zig-strings-call-c-code/) -  [Michael Lynch](https://mtlynch.io/)
* [How to use hash map contexts to save memory when doing a string table](https://zig.news/andrewrk/how-to-use-hash-map-contexts-to-save-memory-when-doing-a-string-table-3l33) - [Andrew Kelley](https://zig.news/andrewrk)
* [Zig / Strings in 5 minutes](https://www.huy.rocks/everyday/01-04-2022-zig-strings-in-5-minutes) - [Huy](https://www.huy.rocks/)
* [Pointers in Zig](https://www.nmichaels.org/zig/pointers.html) -  [Nathan](https://www.nmichaels.org/)

### Syntax Extensions

* [Zig Metaprogramming](https://ikrima.dev/dev-notes/zig/zig-metaprogramming/) - ikrima
* [Supercharging Python Performance with Zig: Building Python Packages and Benchmarking for Speed](https://www.linkedin.com/pulse/supercharging-python-performance-zig-building-packages-bassem-aziz-glmlc/) - [Bassem Aziz](https://www.linkedin.com/in/bassemaziz/)

### Optional

* [What's up with Zig's Optionals?](https://www.reddit.com/r/ProgrammingLanguages/comments/1bn2i58/whats_up_with_zigs_optionals/) - Reddit
* [Proposal: Optional argument names in function calls](https://github.com/ziglang/zig/issues/982)
* [Ziglang Document:Optionals](https://ziglang.org/documentation/master/#Optionals)

## Playground

* [Zig Playground](https://zig-play.dev/)
* [alternative](https://godbolt.org/)

## Locale links

* [TODO: Chinese](zh_CN.md)

## Connection

Are you searching for a Ziguanas ? [Ziglang.org](https://github.com/zig-community/user-map)

Do you want to ask a question? [Zig Users Forum](https://ziggit.dev/), [Reddit](https://www.reddit.com/r/Zig/)

Do you want to meet them IRL? [Community](https://github.com/ziglang/zig/wiki/Community)

Go to Ziguanas events? [Zig SHOWTIME](https://zig.show/), [Zig conferences and events](https://zig.news/t/conference)

Are you looking for a job? [Zig Jobs on Indeed](https://www.indeed.com/q-zig-programming-jobs.html)

Are you fast, simple, and focused? [Find something Ziggy to work on!](https://github.com/ziglang/zig/issues)

Do you want to stay up to date? [The official blog](https://ziglang.org/news/), [Zig NEWS](https://zig.news/), [The official reddit](https://www.reddit.com/r/Zig/)

Do you want to find out why some historical decisions took place? [Zig GitHub Discussions](https://github.com/ziglang/zig/wiki/FAQ)

### Fearless Zig Bloggers

* [Andrew Kelley](https://github.com/andrewrk) - [blog](https://andrewkelley.me/)
* [Jonathan Marler](https://github.com/marler8997) - [blog](https://marler8997.github.io/)
* [Hejsil](https://github.com/Hejsil) - [blog](https://hejsil.github.io/)
* [Hexops](https://github.com/hexops) - [blog](https://hexops.com/)
* [Karl Seguin](https://www.github.com/karlseguin) - [blog](https://www.openmymind.net)
* [Loris Cro](https://github.com/kristoff-it) - [blog](https://kristoff.it/)
* [tigerbeetle](https://github.com/tigerbeetle/tigerbeetle) - [blog](https://tigerbeetle.com/blog)
* [Validark](https://github.com/Validark) - [blog](https://validark.github.io/)
* [Mitchell Hashimoto](https://github.com/mitchellh) - [blog](https://mitchellh.com/)

## Tutorials & Workshop Materials

These are slides and materials from brick-and-mortar workshops about Zig.
While they're unlikely to help a student learning independently, they may be
of interest if you're running a workshop on Zig.

* Loris Cro's [Ziglings](https://github.com/ratfactor/ziglings), a series of small exercises introducing Zig syntax and concepts interactively.  
* [Zig SHOWTIME Videos](https://zig.show/) featuring tutorials and real-world examples from the Zig community.  
* sleibrock' [Zig and WebAssembly Tutorial](https://dev.to/sleibrock/webassembly-with-zig-part-1-4onm) covering Zig's use in modern WebAssembly projects.  
* [Zig Advent Calendar](https://effectivetypescript.com/2024/07/17/advent2023-zig/) offering a curated set of beginner to advanced Zig tutorials and exercises.  
* orhun's [Zig Bits](https://blog.orhun.dev/zig-bits-01/) focusing on practical library implementation in Zig.  
* [A half-hour to learn Zig](https://gist.github.com/ityonemo/769532c2017ed9143f3571e5ac104e50) this is inspired by [a-half-hour-to-learn-rust](https://fasterthanli.me/blog/2020/a-half-hour-to-learn-rust/)
* [A Unix Shell in Zig](https://ratfactor.com/zig/forking-is-cool) exploration combining Zig with scripting tools.
