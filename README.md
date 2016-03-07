# Google Dart Language

This tutorial describes the necessary steps to develop Dart applications.

## Install environment (Dart SDK + Stagehand + Dartium + Atom)

**Install Dart SDK on Linux:**  
https://www.dartlang.org/downloads/linux.html

**Install Dartium browser:**

The Dartium browser is a hacked version of Chromium able to run Dart scripts natively:   https://www.dartlang.org/tools/dartium/

**Install `stagehand` utility:**  

Stagehand is a command line utility to create basic layouts:  
https://github.com/google/stagehand

The following command list all available layouts:  
```bash
# list basic layouts
> stagehand
```

**Install Atom editor**

Download and install Atom:  
https://atom.io/

Install dartlang plugin:  
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
