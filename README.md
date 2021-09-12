# COMP3111/H on VSCode

For those whose doesn't like Eclipse...

**This repository aims to be a reference for myself and those who like to use VSCode's devcontainer (aka Docker) to develop for the course's Labs and Project.**
If you don't know either of them, this repo is possibly not for you.

Feel free to post PRs or Issues.

## Current Progress

The setup works perfectly as of Lab1.

## Brief Introduction

VSCode's devcontainer uses Docker to provide an isolated development environment.

Ecplise uses `Gradle` as its build system, which in itself is cross-platform, provides a cli interface, and can be used on VSCode.

## Our Goal

Use VSCode to develop project that is compatible with Eclipse's build system.

## Prerequisite

### With Container

* Eclipse (only to initialize project)
* VSCode with `Remote - Containers` installed
* Docker

### Without Container

* Eclipse (only to initialize project)
* Correct version of openJDK in your `$PATH`
* VSCode with `Extension Pack for Java` installed

## Project Initialization

### With Devcontainer

#### Quick Version

* Initialize the project in Eclipse or downlord the skeleton from canvas
* If you used VSCode's devcontainer before, just copy the folder `.devcontainer` to your project folder. Rest should be familiar.

#### Long Version

* Read https://code.visualstudio.com/docs/remote/containers-tutorial first, then follow the quick version.

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
