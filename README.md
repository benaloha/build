# Tensorflow build

## Original Readme
[Original README](README1.md)

## RPI crosscompile
[Build for RPI](raspberry_pi_builds/README.md)

## Blog
https://www.bitsy.ai/3-ways-to-install-tensorflow-on-raspberry-pi/

## Build

### Download the TensorFlow source code

Use [Git](https://git-scm.com/) to clone the
[TensorFlow repository](https://github.com/tensorflow/tensorflow):

```
git clone https://github.com/tensorflow/tensorflow.git
cd tensorflow
```

The repo defaults to the `master` development branch. You can also checkout a
[release branch](https://github.com/tensorflow/tensorflow/releases)
to build:

```
git checkout v2.4.0
```

### Build cmd

```
tensorflow/tools/ci_build/ci_build.sh PI-PYTHON38 \
    tensorflow/tools/ci_build/pi/build_raspberry_pi.sh AARCH64
```

This takes 2 hrs on my PC (Intel i7)
