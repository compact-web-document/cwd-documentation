# Compact Web Document documentation

This repository will hold all documentation resources and help & tricks in order to get all setup and ready to use.

## The structure of the project

The CWD repositories are distributed as follows:

- `cwd-reader` - Cross platform GUI reader for the CWD format
- `cwd-lib` - Core of CWD that includes all manipulation of the document API
- `cwd-integrations` - Some example of integration of the CWD lib
- `cwd-editor` - Document editor and creator for the CWD format
- `cwd-app` - Cross platform mobile application
- `cwd-assets` - Assets, resources, graphics and more
- `cwd-site-frontend` - Frontend for the CWD public site
- `cwd-site-backend` - Web Services for the CWD public site
- `cwd-test` - Automated testing suite for all the libraries and CWD repositories

## Building

If you want a minimal environment where you can play with the CWD format, act as follows:

- Create a `cwd` folder where you'll put all project repositories
- Enter on the `cwd` folder
- Clone this repository
- Clone the [cwd-lib](https://github.com/compact-web-document/cwd-lib) repository
- Clone the [cwd-reader](https://github.com/compact-web-document/cwd-reader) repository

These are the minimal needed projects for let CWD running.

### Linux (Ubuntu)

Prepare your environment installing all WebKit and relative needed libraries such:

- `sudo apt install libwebkit2gtk-4.0-dev`
- `sudo apt install libgtk-3-dev`
- `sudo apt install libsoup2.4-dev`

Install the needed Rust binaries and tools:

- `curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`

### MacOS

Prepare your environment installing all WebKit and relative needed libraries such:

- `brew install webkitgtk`
- `brew install gtk+3` or `brew install gtk+`
- `brew install libsoup`

Install the needed Rust binaries and tools:

- `curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`

### Windows (TODO)

Prepare your environment installing all WebKit and relative needed libraries such:

- Download and link to MiniGW [this](https://github.com/webview/webview/tree/master/dll/x64) library folder

Install the needed Rust binaries and tools:

- Download Rust [here](https://win.rustup.rs/x86_64)

## Running

First of all, you need to build the `cwd-lib` library, you can do it with `cargo +stable build` inside the `cwd-lib` folder. Once you do that, the library will be available for the Reader embedding.

Second, you have to build the `cwd-reader` in order to play with the CWD file, please install [CLion EAP](https://www.jetbrains.com/clion/nextversion/) and then open the `cwd-reader` project and simply run it.

If everything is setup correctly, you will see something like:

![CWD Reader](assets/screenshot.png)