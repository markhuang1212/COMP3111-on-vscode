# COMP3111/H on VSCode

For those whose doesn't like Eclipse...

Some programmers (such as me) doesn't like to use IDE, especially when faced with Eclipse with a laggy, overcomplicated and unintuitive UI (no offense!). 
Yet that's what HKUST kind of forced us to do (once on COMP1022P, COMP201(1|2) now on COMP3111/H).
**This repository aims to be a reference for myself and those who like to use VSCode's devcontainer (aka Docker) to develop for the course's Labs and Project.**
If you don't know either of them, this repo is possibly not for you.

Feel free to post PRs or Issues.

## Brief Introduction

VSCode's devcontainer uses Docker to provide an isolated development environment. Microsoft provides an out-of-the-box devcontainer for Java.

Ecplise uses `Gradle` as its build system, which in itself is cross-platform, provides a cli interface, and can be used on VSCode.

## Our Goal

Use VSCode to develop project that is compatible with Eclipse's build system.

## Prerequisite

* A x86 Computer
* Docker for Linux/Windows/Mac
* VSCode with the extension "Remote - Containers" installed
* Familarity with VSCode and Docker

## Project Initialization

### Lab 1

1. Create a folder called `lab1`, open it in VSCode.
2. Open Command Line Palette (Command+Shift+P), Select `Remote-Containers: Add Development Containers Configuration Files`, Select `Java`, Select `16`, select `none`, select `Install Maven` and `Install Gradle`.
3. Open Command Line Palette and select `Remote-Containers: Open Folder in Containers`, select the current folder
4. Wait for container to build, it will take a few minutes for the first time.
5. In the VSCode's terminal, run `gradle init`, select `2: application` and `3: java` in corresponding questions. Press `enter` in other questions to use the default.
6. Wait for about half a minute to let the Java Extension to do its job.
7. Good to go! You can now build, test and debug in VSCode.

## License

MIT

## Disclaimer

This is not a tutorial, use it at your own risk.
