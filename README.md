# VS Code MicroProfile Rest Client Generator Extension

[![Marketplace Version](https://vsmarketplacebadge.apphb.com/version/MicroProfile-Community.mp-rest-client-generator-vscode-ext.svg "Current Release")](https://marketplace.visualstudio.com/items?itemName=MicroProfile-Community.mp-rest-client-generator-vscode-ext)
[![Build Status](https://travis-ci.org/MicroShed/mp-starter-vscode-ext.svg?branch=master)](https://travis-ci.org/MicroShed/mp-rest-client-generator-vscode-ext)

The MicroProfile REST Client Generator Extension provides support for generating a [MicroProfile](https://microprofile.io/) REST Client interface template from an [OpenAPI](https://github.com/OAI/OpenAPI-Specification) document. This extension calls the [openapi-generator](https://github.com/OpenAPITools/openapi-generator) to generate `models` and `apis` folders. The code for this extension is hosted under the MicroShed organization on GitHub. Learn more about MicroProfile REST Client on [GitHub](https://github.com/eclipse/microprofile-rest-client).

![Open Liberty Tools Extension](images/RestClientExtension.png)

## Quick Start

- Install the extension
- Launch the VS Code command palette `(View -> Command Palette...)`, then select `MicroProfile: Generate a MicroProfile REST Client` to run the extension

## Input

The extension prompts for the following parameters:

1. Path or url to an OpenAPI document
2. `src` directory of project to generate into
3. Package name

The extension will generate `models` and `apis` folders into the specified directory. The package name will be auto-filled based on the directory generated into.

## Contributing

Contributions to the MicroProfile REST Client Generator extension are welcome!

Our [CONTRIBUTING](CONTRIBUTING.md) document contains details for submitting pull requests.

To build and run the extension locally:

1. `git clone git@github.com:MicroShed/mp-rest-client-generator-vscode-ext.git`
2. `cd mp-rest-client-generator-vscode-ext`
3. `npm install`
4. Run the extension in VS Code by selecting `Run Extension` from the debug panel or by pressing `F5`

   Alternatively, build a `.vsix` file:

   - Run `vsce package` to generate the `mp-rest-client-generator-vscode-ext-xxx.vsix` file
   - Install the extension to VS Code by `View/Command Palette`
   - Select `Extensions: Install from VSIX...` and choose the generated `mp-rest-client-generator-vscode-ext-xxx.vsix` file

## Issues

Please report bugs, issues and feature requests by creating a [GitHub issue](https://github.com/MicroShed/mp-rest-client-generator-vscode-ext/issues).
