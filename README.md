#  [MediaPipe](https://github.com/google/mediapipe) for Apple Silicon
Prebuilt Google MediaPipe packages for Apple Silicon (`arm64`).

## Install
To install the prebuilt packages, use the following command. The package is called **mediapipe-silicon** but is a drop-in-replacement for the mediapipe package.

```
pip install mediapipe-silicon --find-links https://github.com/cansik/mediapipe-silicon/releases/tag/v0.8.9
```

## Build
To build the libraries yourself, please first install the following dependencies and run the build script.

```
brew install wget cmake protobuf bazelisk opencv@3
brew uninstall --ignore-dependencies glog
```

```
./build-macos.sh
```

The pre-built wheel packages should be in the `dist` directory.

## About
MIT License - Copyright (c) 2022 Florian Bruggisser