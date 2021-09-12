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

### General Approach

1. Initialize a project in Eclipse as spcified by the Lab requirement, or download the skeleton code that is provided.
    * This step can also be skipped if you know how to use `Gradle` via command line.
2. Copy all the files to a seperate folder and open the folder in VSCode.
3. Open Command Palette (Command+Shift+P), Select `Remote-Containers: Add Development Containers Configuration Files`, Select `Java`, Select `16`, select `none`, select `Install Maven` and `Install Gradle`.
4. Open Command Palette and select `Remote-Containers: Open Folder in Containers`, select the current folder
    * If VSCode asks you whether to open the current folder in Container, just select `yes`.
5. Wait for container to build, it will take a few minutes for the first time.
6. If VSCode ask `Do you want xxx to configure java automatically`, always select `yes`.
7. You are good to go!

If anything bad happen, you can always select `Rebuild Container` in the Command Palette.

For Git Graphs, you can install the extension "Git Graph" in your VSCode container.

## License

MIT

## Disclaimer

This is not a tutorial, use it at your own risk.
