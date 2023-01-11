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

# What's Here?

This repo includes:

- The code examples from the [Getting Started section](https://crystal-lang.org/reference/1.7/getting_started/index.html) of the Crystal website are here..

```
.
├── LICENSE                     # a lovely MIT license file
├── README.md                   # the README.md that you're currently reading
└── getting_started             # the examples from Getting Started on https://crystal-lang.org/
    ├── all_my_cli.cr
    ├── hello_goodbye.cr
    ├── hello_world.cr
    ├── help.cr
    ├── http_server.cr
    ├── let_it_cli_1.cr
    ├── let_it_cli_2.cr
    ├── let_it_cli_colour.cr
    ├── twist_and_shout.cr
    └── yellow_cli.cr
```

# Notes and Comments

I was surprised by just how many packages I needed to install to get this Ubuntu container set up so that the Crystal samples would run. You can see the list in `Dockerfile`.

The blinking CLI example didn't blink. I wonder if that's a limitation of the containerised Ubuntu bash shell within VS Code.

