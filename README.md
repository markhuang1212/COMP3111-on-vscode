# COMP3111/H on VSCode

For those whose doesn't like Eclipse...

Some programmers (such as me) doesn't like to use IDE, especially when faced with Eclipse with a laggy, overcomplicated and unintuitive UI (no offense!). 
Yet that's what HKUST kind of forced us to do (once on COMP1022P, COMP201(1|2) now on COMP3111/H).
**This repository aims to be a reference for myself and those who like to use VSCode's devcontainer (aka Docker) to develop for the course's Labs and Project.**
If you don't know either of them, this repo is possibly not for you.

Feel free to post PRs or Issues.

## TODO

It turns out that Microsoft's Java container doesn't support Java15, so I will write my own in the following days. For now, only the non-container version is supported.

## Brief Introduction

VSCode's devcontainer uses Docker to provide an isolated development environment.

Ecplise uses `Gradle` as its build system, which in itself is cross-platform, provides a cli interface, and can be used on VSCode.

## Our Goal

Use VSCode to develop project that is compatible with Eclipse's build system.

## Prerequisite

### With Container

TBA

### Without Container

* Eclipse (only to initialize project)
* Correct version of openJDK in your `$PATH`
* VSCode with `Extension Pack for Java` installed

## Project Initialization

### With Devcontainer

TBA

### Without Container

* Install VSCode's Java Extension Pack
* Initialize the project in Eclipse or downlord the skeleton from canvas
* Open the project in VSCode
* If VSCode asks questions like `do you want to configure Java automatically`, always select `yes`
* You are good to go!

## License

MIT

## Disclaimer

This is not a tutorial, use it at your own risk.
