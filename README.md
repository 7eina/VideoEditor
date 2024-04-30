# Video Editor

## Overview
This project is a C++ application for managing and editing videos and their associated scenes. It provides an interface for creating videos, adding scenes, and storing videos in a repository.

Created: Summer 2023

## Compatibility
- **Ubuntu**: This software is fully compatible with Ubuntu. It can be compiled and executed in any standard Ubuntu environment.
- **Virtual Box on Linux**: The software can also be run on Linux distributions installed within Virtual Box. Ensure that your Virtual Box setup has adequate resources allocated for smooth operation.
- **CLion on Windows**: The project can be loaded and executed in the CLion IDE on Windows. This requires a C++ environment setup in CLion, including the MinGW or Cygwin toolchains.

## System Requirements
- **Linux**: GCC compiler and standard C++ libraries.
- **Windows**: CLion with MinGW or Cygwin.

## File Structure
- `defs.h`: Definitions and constants used across the application.
- `Date.h`/`Date.cc`: Manages date information for scenes.
- `Scene.h`/`Scene.cc`: Entity object that contains data for a scene, including title, date, and content.
- `SceneArray.h`/`SceneArray.cc`: Collection object that serves as a data structure for managing scenes.
- `Video.h`/`Video.cc`: Entity object that contains video information including title, description, and manages scene collections.
- `VideoArray.h`/`VideoArray.cc`: Collection object that serves as a data structure for managing videos.
- `VideoRepo.h`/`VideoRepo.cc`: Manages video collections and provides features to access, save, delete, and play videos.
- `Editor.h`/`Editor.cc`: Connects to a `VideoRepo` object to save or download the current video, add or remove scenes from the video, and print error messages.
- `TestView.h`/`TestView.cc`: Presents a menu and takes input from the user for performing tests.
- `TestControl.h`/`TestControl.cc`: Controls the running of tests on the application, interacting with `TestView`.
- `main.cc`: The main entry point for the application.
- `Makefile`: Specifies the set of tasks to be executed by the `make` command.
- `README.txt`: This documentation file.

## Compilation and Execution

### Compile
To compile the application, open a terminal window in the project directory and enter the following command:
```bash
make
```

### Execute
To run the application, use the command:
```bash
./main
```
