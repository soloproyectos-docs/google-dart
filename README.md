# Google Dart Language
Google Dart Language, considerations an tutorial.

Install [Dart SDK](https://www.dartlang.org/tools/sdk/)

## Install Dartium

Dartium is a version of the Chromium explorer able to execute natively dart code: [Dartium](https://www.dartlang.org/tools/dartium/)

## Stagehand

A script to create basic project layouts: [Stagehand](https://github.com/google/stagehand)

For example:
```bash
// creates a basic web layout in the current directory
> stagehand web-simple
```

## Dart Editor

[Atom](https://atom.io/) is a good and free editor. And it has support for Dart:  
https://github.com/dart-atom/dartlang

## Your first web application

You can use [stagehand](https://github.com/google/stagehand) and [pub get](https://www.dartlang.org/tools/pub/cmd/pub-get.html) to create a basic web layout and install dependencies:
```bash
# creates a simple web layout
> stagehand web-simple
# install dependences
> pub get
```

Use [pub build](https://www.dartlang.org/tools/pub/cmd/pub-build.html) to deploy your application:
```bash
# the following command creates a build directory with necessary assets
> pub build
```

You can find more info about the `pub` command at:  
https://www.dartlang.org/tools/pub/get-started.html
https://www.dartlang.org/tools/pub/cmd/
