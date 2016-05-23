# Google Dart Language

This tutorial describes the necessary steps to prepare your computer to develop Dart applications.

## Install environment (Dart SDK + Stagehand + Dartium + Atom)

**Install Dart SDK on Linux:**  
https://www.dartlang.org/downloads/linux.html

Dart SDK is probably installed in `/usr/lib/dart`. Add the following line to the ~/.profile file:
```bash
# Dart SDK binaries directory
> export PATH="$PATH:/usr/lib/dart/bin"
```

**Install `stagehand` utility:**  

Stagehand is a command line utility to create basic layouts:  
https://github.com/google/stagehand

After installing `stagehand`, you may need to add the following line to your ~/.profile file:
```bash
# Pub bin directory
> export PATH="$PATH":"~/.pub-cache/bin"
```

The following command prints all available layouts:  
```bash
# prints basic layouts
> stagehand
```

**Install Dartium browser:**

The Dartium browser is a hacked version of Chromium able to run Dart natively:  
https://www.dartlang.org/tools/dartium/

**Install Atom editor**

There are several IDEs to create Dart applications. But I'd recommend using Atom Editor, because it's nice and it's free. However, you can use another editor:  
https://www.dartlang.org/tools/

Download and install Atom:  
https://atom.io/

Install `dartlang` plugin:  
https://github.com/dart-atom/dartlang

Go to the `dartlang` settings and selects the "[Experimental] Format files on save" option. This option invokes the [dartfmt](https://github.com/dart-lang/dart_style) command when the files are saved.

## Create, install, run and compile projects

Use the [pub](https://pub.dartlang.org/) package manager to install dependences, compile and run Dart applications.

**Crate a simple web project**
```bash
# change to the project path
> cd path/to/project

# create a simple web project in the current directory
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

**Compile or build the project to be executed sucessfully in other browser**:
```bash
# create a 'build' directory with the necessary assets (JavaScript files, etc...)
> pub build
```

## Notes

If you want to run a Dart application in your mobile device, execute the following code:
```bash
# open http://<computer-ip>:8080 in any external device
pub server --hostname=<computer-ip>
```
