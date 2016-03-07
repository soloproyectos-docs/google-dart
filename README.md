# Google Dart Language
Google Dart Language, considerations an tutorial.

Install [Dart SDK](https://www.dartlang.org/tools/sdk/)

## Install environment (Dart SDK + Stagehand + Dartium + Atom)

**Install Dart SDK on Linux:**  
https://www.dartlang.org/downloads/linux.html

**Install Dartium browser:**

Dartium is a version of the Chromium explorer able to execute natively dart code: [Dartium](https://www.dartlang.org/tools/dartium/)

### Install `stagehand` utility

A script to create basic project layouts: [Stagehand](https://github.com/google/stagehand)

For example:
```bash
// creates a basic web layout in the current directory
> stagehand web-simple
```

### Install a Dart editor

[Atom](https://atom.io/) is a good and free editor. And it has support for Dart:  
https://github.com/dart-atom/dartlang

## Create, install, run and compile projects

Use the [pub](https://pub.dartlang.org/) package manager to install dependences, compile and run a `dart` server.

**Crate a simple web project**
```bash
# change to the project path
> cd path/to/project

# create a simple web project
> stagehand web-simple
```

**Install dependences**:
```bash
# install (or get) dependences
> pub get
```

**Run the project in the Dartium browser (localhost:8080)**:
```bash
# run dart server (open localhost:8080 in the Dartium browser)
> pub serve
```

**Compile or build the project to be executed sucessfully in normal browser**:
```bash
# this creates the 'build' directory with necessary assets (JavaScript files, etc...)
> pub build
```
