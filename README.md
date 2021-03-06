# Docker + Alpine + Node = Love

This Dockerfile provides a good base build image to use in multistage builds for Node apps. It comes with the latest version of Alpine, Node and NPM. It is intended for use in creating release images with or for your application and allows you to avoid cross-compiling releases. The exception of course is if your app has dependencies which require a native compilation toolchain, but that is an exercise left to the user.

No effort has been made to make this image suitable to run in unprivileged environments. The repository owner is not responsible for any losses that result from improper usage or security practices, as it is expected that the user of this image will implement proper security practices themselves.

## Software/Language Versions

```shell
Alpine 3.12.0
Nodejs 14.5.0
NPM 6.14.6
```

## Usage

To boot straight to a node prompt in the image:

```shell
$ docker run --rm -i -t beardedeagle/alpine-node-builder node
Welcome to Node.js v14.5.0.
Type ".help" for more information.
>
```
