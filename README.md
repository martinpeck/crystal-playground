# Crystal Playground

Somewhere to play with the Crystal programming language.

This repository contains a [VS Code](https://code.visualstudio.com/) [Dev Container](https://containers.dev/) that installs [Crystal](https://crystal-lang.org/), and its various dependencies, into an Ubuntu container.

If you open this folder in VS Code, and have the Dev Container extension, you will end up with a container-based environment where you can then run commands such as...

```
$ crystal --version
Crystal 1.7.0 [016578f85] (2023-01-09)

LLVM: 13.0.1
Default target: x86_64-unknown-linux-gnu
```

The Dev Container will also have the VS Code Extension for Crystal installed.

# How is Crystal Installed?

Good question. It's installed as a [Dev Container Feature using the asdf package](https://github.com/devcontainers-contrib/features/tree/main/src/crystal-asdf) (see `./.devcontainer/devcontainer.json`)


