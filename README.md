# devonfw VS Code extensions

The extensions included in this pack involve several aspects as Remote Development, Team Collaboration, Project Management, devonfw projects development, support for other interesting languages and technologies, code running, testing, linting and IDE configuration:

- Remote Development
  - [Visual Studio Code Remote Development Extension Pack](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)
- Team Collaboration
  - [VS Live Share Extension Pack](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare-pack)
    - Please read the following instructions https://docs.microsoft.com/en-us/visualstudio/liveshare/use/vscode
- Settings Sync
  - [Settings Sync](https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync)
- Project Management
  - [Project Manager](https://marketplace.visualstudio.com/items?itemName=alefragnani.project-manager)
- Code and documentation helpers
  - [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
  - [Bracket Pair Colorizer](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer)
  - [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
    - In order to avoid TS lint errors, you must set the `prettier.singleQuote` and `prettier.semi` variables to `true` in the VS Code User Settings (Keyboard shortcut `Ctrl+,` in Windows and Linux or `Cmd+,` in macOS or press `F1` and start writing _User settings_).
    - Another useful feature to avoid TS lint errors is to set the `prettier.trailingComma` variable to `all` to trail commas wherever possible.
    - Besides this, a `.prettierrc` JSON file can be included in the root folder of any Angular project with the following configuration:
    ```json
    {
      "singleQuote": true,
      "trailingComma": "all",
      "arrowParens": "always",
      "semi": true
    }
    ```
    - Last but not least, the prettier configuration can be also included in every JavaScript/TypeScript project inside the `package.json` file adding its own key:
    ```json
    "prettier": {
      "singleQuote": true,
      "trailingComma": "all",
      "arrowParens": "always",
      "semi": true
    }
    ```
    - Refer to the official documentation https://prettier.io/docs/en/configuration.html for further details.
  - [Document This](https://marketplace.visualstudio.com/items?itemName=joelday.docthis)
  - [Search Docsets](https://marketplace.visualstudio.com/items?itemName=silverlakesoftware.searchdocsets-vscode)
  - [TODO Highlight](https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight)
  - [FreeMarker](https://marketplace.visualstudio.com/items?itemName=dcortes92.FreeMarker)
  - [Polacode](https://marketplace.visualstudio.com/items?itemName=pnp.polacode)
    - Please follow the instructions to configure properly this extension.
  - [Dependency Analytics](https://marketplace.visualstudio.com/items?itemName=redhat.fabric8-analytics)
    - This extension assumes that you have the binaries `npm` and `mvn` on your PATH.
  - [PrintCode](https://marketplace.visualstudio.com/items?itemName=nobuhito.printcode)
- Code runners
  - [Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner)
  - [Quokka.js](https://marketplace.visualstudio.com/items?itemName=WallabyJs.quokka-vscode)
- Angular, Ionic, React Native, NativeScript and TypeScript
  - [Angular Snippets](https://marketplace.visualstudio.com/items?itemName=johnpapa.Angular2)
  - [Angular Language Service](https://marketplace.visualstudio.com/items?itemName=Angular.ng-template)
  - [ES7 React/Redux/GraphQL/React-Native snippets](https://marketplace.visualstudio.com/items?itemName=dsznajder.es7-react-js-snippets)
  - [React Native Tools](https://marketplace.visualstudio.com/items?itemName=msjsdiag.vscode-react-native)
  - [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
  - [TSLint](https://marketplace.visualstudio.com/items?itemName=ms-vscode.vscode-typescript-tslint-plugin)
  - [Ionic Snippets](https://marketplace.visualstudio.com/itemdetails?itemName=fivethree.vscode-ionic-snippets)
  - [NativeScript](https://marketplace.visualstudio.com/items?itemName=Telerik.nativescript)
  - [Cordova Tools](https://marketplace.visualstudio.com/items?itemName=vsmobile.cordova-tools)
  - [NgRx Snippets](https://marketplace.visualstudio.com/itemdetails?itemName=hardikpthv.NgRxSnippets)
  - [Jest](https://marketplace.visualstudio.com/items?itemName=Orta.vscode-jest)
- CSS
  - [CSS Peek](https://marketplace.visualstudio.com/items?itemName=pranaygp.vscode-css-peek)
- Debuggers
  - [Debugger for Chrome](https://marketplace.visualstudio.com/items?itemName=msjsdiag.debugger-for-chrome)
- Git
  - [Git History](https://marketplace.visualstudio.com/items?itemName=donjayamanne.githistory)
  - [GitLens — Git supercharged](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
  - [GitHub Pull Requests](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github)
- Swagger and API definition
  - [OpenAPI (Swagger) Editor](https://marketplace.visualstudio.com/items?itemName=42crunch.vscode-openapi)
  - [REST Client](https://marketplace.visualstudio.com/items?itemName=humao.rest-client)
- UML
  - [PlantUML](https://marketplace.visualstudio.com/items?itemName=jebbs.plantuml)
- Rust
  - [Rust (rls)](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust)
- Python
  - [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
- C++
  - [C/C++](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools)
- C#
  - [C#](https://marketplace.visualstudio.com/items?itemName=ms-vscode.csharp)
- Java
  - [Java Extension Pack](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack) that will install automatically:
    - [Language Support for Java(TM) by Red Hat](https://marketplace.visualstudio.com/items?itemName=redhat.java)
    - [Debugger for Java](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-debug)
    - [Java Test Runner](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-test)
    - [Maven for Java](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-maven)
  - The following extensions add support and tools to develop **Spring Boot** Java applications:
    - [Spring Boot Dashboard](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-spring-boot-dashboard)
    - [Spring Boot Tools](https://marketplace.visualstudio.com/items?itemName=Pivotal.vscode-spring-boot)
    - [Spring Initializr Java Support](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-spring-initializr)
  - In order to make Java work properly you must set the `java.home` variable in the VS Code User Settings (Keyboard shortcut `Ctrl+,` in Windows and Linux or `Cmd+,` in macOS or press `F1` and start writing _User settings_)
- Key bindings
  - [Sublime Text Keymap and Settings Importer](https://marketplace.visualstudio.com/items?itemName=ms-vscode.sublime-keybindings)
- Docker
  - [Docker](https://marketplace.visualstudio.com/items?itemName=PeterJausovec.vscode-docker)
- Themes
  - [Cobalt2 Theme Official](https://marketplace.visualstudio.com/items?itemName=wesbos.theme-cobalt2) - Press F1, choose **Color Theme** option and select **Cobalt**.
  - [Noctis - collection of light & dark themes](https://marketplace.visualstudio.com/items?itemName=liviuschera.noctis) - Press F1, choose **Color Theme** option and select one of multiple schemes beginning with **Noctis**.
  - [vscode-icons](https://marketplace.visualstudio.com/items?itemName=robertohuertasm.vscode-icons) - Press F1, choose **File Icon Theme** option and select **VSCode Icons**.
- Spell checking
  - [SpellChecker](https://marketplace.visualstudio.com/items?itemName=swyphcosmo.spellchecker)
- AsciiDoc
  - [AsciiDoc](https://marketplace.visualstudio.com/items?itemName=asciidoctor.asciidoctor-vscode)
- XML
  - [XML](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-xml)
- YAML
  - [YAML](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-yaml)
- Miscellaneous
  - [LineCount](https://marketplace.visualstudio.com/items?itemName=yycalm.linecount)
  - [Lorem ipsum](https://marketplace.visualstudio.com/items?itemName=Tyriar.lorem-ipsum)
  - [Resource Monitor](https://marketplace.visualstudio.com/items?itemName=mutantdino.resourcemonitor)
  - [Draw.io Diagram Editor](https://marketplace.visualstudio.com/items?itemName=hediet.vscode-drawio)
    - Embeddded version of the Draw.io graphical diagram editor. Uses an offline version of Draw.io by default.

## Requirements

### Microsoft Visual Studio Code

In order to install this package **Microsoft Visual Studio Code 1.35.0** at least must be installed. It is recommended to upgrade VS Code in any case.

### C/C++ support

See [C/C++ for Visual Studio Code](https://code.visualstudio.com/docs/languages/cpp) for a Guide on how to configure and use the extension enabling C/C++ support for Visual Studio Code. This provides support for cross-platform C and C++ development using VS Code on Windows, Linux, and macOS.

### AsciiDoc support

AsciiDoc extension comes with Asciidoctor.js library for preview bundled. If you want to use the Ruby version of Asciidoctor you need to change the `AsciiDoc.use_asciidoctor_js` setting to false.

In order to be able to use the AsciiDoc Ruby version you have to install **Ruby** on your system and the **Asciidoctor** tool running the following command in the terminal:

```bash
$ gem install asciidoctor
```
