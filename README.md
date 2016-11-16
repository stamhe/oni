# Oni
## Neovim + JavaScript powered IDE

- [Introduction](#Introduction)
- [Usage](#Usage)
- [Roadmap](#Roadmap)
- [User Guide](#User Guide)
- [Extension Points](#Extension Points)
- [License](#License)
- [Contributing](#Contributing)
- [Thanks](#Thanks)

## Introduction

ONI is a NeoVim front-end UI with rich IDE-like UI integration points.

This repository is under __active development__, and until 1.0 please consider everything unstable.

## Usage

- For Windows, a pre-built x86 binary of NeoVim is included for convenience.

- For OSX, there is no included pre-built binary. Please [Install Neovim](https://github.com/neovim/neovim/wiki/Installing-Neovim) and ensure the 'nvim.exe' is available.

1) Clone the repository

`git clone TODO`

2) Install dependencies by running `npm install` from the root
3) Build using 'npm run build' from the root
4) Run `npm link` to register the *ONI* command
5) Run `oni` at the command line

## Goals

The goal of this project is to provide both the full-fledged VIM experience, with no compromises, while pushing forward to enable new scenarios.

- __Rich plugin development__ - using JavaScript, instead of VimL, allowing deep-language integration.
- __Cross-platform support__ - across OS X and Windows.
- __Batteres included__ - rich features are available out of the box. TypeScript development is the canonical example, but the hope is that other language providers will be included. Later, an included package manager will make it simple to find and install plugins.
- __Performance__ - no compromises, VIM is fast, and ONI should be fast too.
- __Ease Learning Curve__ - without sacrificing the VIM experience

VIM is an incredible tool for manipulating *text* at the speed of thought. With a composable, modal command language, it is no wonder that VIM usage is still prevalent today even in the realm of modern editors.

However, going from thought to *code* has some different challenges than going from thought to *text*. IDEs today provide several benefits that help to reduce __cognitive load__ when writing code, and that benefit is tremendously important - not only in terms of pure coding efficiency and productivity, but also in making the process of writing code enjoyable and fun.

In my journey of learning VIM and increasing proficiency in other editors, I've found there is always a trade-off - either enjoy the autocompletion and IDE features, and compromise on the experience and muscle memory I've built with VIM, or work in VIM and compromise on the rich language functionality we have in an IDE.

The goal of this project is to give an editor that gives the best of both worlds - the power, speed, and flexibility of using VIM for manipulating text, as well as the rich tooling that comes with an IDE.

## Roadmap

- 0.1
    -[x] Initial repo
    -[x] OS X / Windows support
    -[x] TypeScript language support
- 0.2
    -[] Mouse support
        -[] Buffer scroll bars
    -[] Extensibility models
        -[] Language service
            -[] Autocompletion (TypeScript, Javascript)
            -[] QuickInfo (TypeScript, JavaScript)
            -[] Goto Definition (TypeScript, JavaScript)
            -[] Errors
    -[] Services
        -[] QuickOpen - Modern CTRL-P replacement
    -[] Installation via NPM
- 0.3
    -[] Proper keymap support
    -[] Configuration loading
    -[] Git overlays
    -[] QuickOpen Improvements
        -[] Non-git strategy
        -[] Fuzzy Matching
        -[] Scrollbar
    -[] AutoCompletion
        -[] Fuzzy Matching
        -[] Scrollbar

- Future
    -[] Icon
    -[] Scrollbar minimap (a-la sublime)
    -[] Enhanced VimTutor
    -[] Debugger support
    -[] Snippet support
    [] Project templates
    [] Package Manager

## Extension Points

TODO: Coming soon. See the oni-typescript implementation for the time being.

### Language Extensibility

### Diagnostic Providers

### Overlays

### Panes

### Debuggers

### Project Templates

### Snippets

## Included VIM Plugins

This distribution contains several VIM plugins that enhance the VIM experience.

These are:
- [targets.vim](https://github.com/wellle/targets.vim)
- [typescript-vim](https://github.com/leafgarland/typescript-vim)
- [vim-commentary](https://github.com/tpope/vim-commentary)

As well as some color-schemes:
- [vim-monokai](https://github.com/sickill/vim-monokai)
- [onedark.vim](https://github.com/joshdick/onedark.vim)

## License

MIT

## Contributing

Contributions are very much welcome :)

# Thanks

Big thanks to the NeoVim team - without their work, this project would not be possible. The deep integration with VIM would not be possible without the incredible work that was done to enable the msgpack-RPC interface. Thanks!

In addition, there are several other great NeoVim front-end UIs [here](https://github.com/neovim/neovim/wiki/Related-projects) that served as great reference points and learning opportunities.