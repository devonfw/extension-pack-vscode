# devonfw VS Code extensions

The extensions included in this pack involve several aspects as Remote Development, Team Collaboration, Project Management, devonfw projects development, support for other interesting languages and technologies, code running, testing, linting and IDE configuration:

- Remote Development
  - [Visual Studio Code Remote Development Extension Pack](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)
- Team Collaboration
  - [VS Live Share Extension Pack](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare-pack)
    - Please read the following instructions <https://docs.microsoft.com/en-us/visualstudio/liveshare/use/vscode>
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

    - Refer to the official documentation <https://prettier.io/docs/en/configuration.html> for further details.

  - [Document This](https://marketplace.visualstudio.com/items?itemName=joelday.docthis)
  - [Search Docsets](https://marketplace.visualstudio.com/items?itemName=silverlakesoftware.searchdocsets-vscode)
  - [TODO Highlight](https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight)
  - [FreeMarker](https://marketplace.visualstudio.com/items?itemName=dcortes92.FreeMarker)
  - [Polacode](https://marketplace.visualstudio.com/items?itemName=pnp.polacode)
    - Please follow the instructions to configure properly this extension.
  - [Dependency Analytics](https://marketplace.visualstudio.com/items?itemName=redhat.fabric8-analytics)
    - This extension assumes that you have the binaries `npm` and `mvn` on your PATH.
  - [PrintCode](https://marketplace.visualstudio.com/items?itemName=nobuhito.printcode)

- Code linting
  - [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
  - [TSLint](https://marketplace.visualstudio.com/items?itemName=ms-vscode.vscode-typescript-tslint-plugin)
  - [SonarLint](https://marketplace.visualstudio.com/items?itemName=SonarSource.sonarlint-vscode)
- Code runners
  - [Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner)
  - [Quokka.js](https://marketplace.visualstudio.com/items?itemName=WallabyJs.quokka-vscode)
- JavaScript and TypeScript
  - [Angular Snippets](https://marketplace.visualstudio.com/items?itemName=johnpapa.Angular2)
  - [Angular Language Service](https://marketplace.visualstudio.com/items?itemName=Angular.ng-template)
  - [ES7 React/Redux/GraphQL/React-Native snippets](https://marketplace.visualstudio.com/items?itemName=dsznajder.es7-react-js-snippets)
  - [React Native Tools](https://marketplace.visualstudio.com/items?itemName=msjsdiag.vscode-react-native)
  - [Ionic Snippets](https://marketplace.visualstudio.com/itemdetails?itemName=fivethree.vscode-ionic-snippets)
  - [Cordova Tools](https://marketplace.visualstudio.com/items?itemName=msjsdiag.cordova-tools)
  - [NgRx Snippets](https://marketplace.visualstudio.com/itemdetails?itemName=hardikpthv.NgRxSnippets)
  - [Jest](https://marketplace.visualstudio.com/items?itemName=Orta.vscode-jest)
  - [Import Cost](https://marketplace.visualstudio.com/items?itemName=wix.vscode-import-cost)
  - [Nx Console](https://marketplace.visualstudio.com/items?itemName=nrwl.angular-console) for **monorepos**. More info at <https://nx.dev/latest/angular/getting-started/console>.
- CSS
  - [CSS Peek](https://marketplace.visualstudio.com/items?itemName=pranaygp.vscode-css-peek)
- Git
  - [Git History](https://marketplace.visualstudio.com/items?itemName=donjayamanne.githistory)
  - [GitLens — Git supercharged](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
  - [GitHub Pull Requests](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github)
  - [Git Graph](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph)
- Swagger and API definition
  - [OpenAPI (Swagger) Editor](https://marketplace.visualstudio.com/items?itemName=42crunch.vscode-openapi)
  - [REST Client](https://marketplace.visualstudio.com/items?itemName=humao.rest-client)
- UML
  - [PlantUML](https://marketplace.visualstudio.com/items?itemName=jebbs.plantuml)
- Rust
  - [Rust (rls)](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust)
- Python
  - [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
  - [Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance)
  - [Jupyter](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)
- C++
  - [C/C++](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools)
- C#
  - [C#](https://marketplace.visualstudio.com/items?itemName=ms-vscode.csharp)
- Java
  - [Java Extension Pack](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack)
  - [Spring Boot Extension Pack](https://marketplace.visualstudio.com/items?itemName=Pivotal.vscode-boot-dev-pack)
  - [Community Server Connectors](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-community-server-connector)
  - [Lombok](https://marketplace.visualstudio.com/items?itemName=GabrielBB.vscode-lombok)
  - In order to make Java work properly you must set the `java.home` variable in the VS Code User Settings (Keyboard shortcut `Ctrl+,` in Windows and Linux or `Cmd+,` in macOS or press `F1` and start writing _User settings_)
  - In order to check the Java extensions for VS Code and test others available you can press F1 and choose **Java: Extension Guide**.
- Key bindings
  - [Sublime Text Keymap and Settings Importer](https://marketplace.visualstudio.com/items?itemName=ms-vscode.sublime-keybindings)
- Docker
  - [Docker](https://marketplace.visualstudio.com/items?itemName=PeterJausovec.vscode-docker)
- Kubernetes
  - [Kubernetes](https://marketplace.visualstudio.com/items?itemName=ms-kubernetes-tools.vscode-kubernetes-tools)
- Themes
  - [Cobalt2 Theme Official](https://marketplace.visualstudio.com/items?itemName=wesbos.theme-cobalt2) - Press F1, choose **Color Theme** option and select **Cobalt**.
  - [Noctis - collection of light & dark themes](https://marketplace.visualstudio.com/items?itemName=liviuschera.noctis) - Press F1, choose **Color Theme** option and select one of multiple schemes beginning with **Noctis**.
  - [GitHub Theme](https://marketplace.visualstudio.com/items?itemName=GitHub.github-vscode-theme) - Press F1, choose **Color Theme** option and select one of multiple schemes beginning with **GitHub**.
  - [vscode-icons](https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons) - Press F1, choose **File Icon Theme** option and select **VSCode Icons**.
- AsciiDoc
  - [AsciiDoc](https://marketplace.visualstudio.com/items?itemName=asciidoctor.asciidoctor-vscode)
- XML
  - [XML](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-xml)
- YAML
  - [YAML](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-yaml)
- Miscellaneous
  - [SpellChecker](https://marketplace.visualstudio.com/items?itemName=swyphcosmo.spellchecker)
  - [LineCount](https://marketplace.visualstudio.com/items?itemName=yycalm.linecount)
  - [Lorem ipsum](https://marketplace.visualstudio.com/items?itemName=Tyriar.lorem-ipsum)
  - [Resource Monitor](https://marketplace.visualstudio.com/items?itemName=mutantdino.resourcemonitor)
  - [Draw.io Diagram Editor](https://marketplace.visualstudio.com/items?itemName=hediet.vscode-drawio)
    - Embedded version of the Draw.io graphical diagram editor. Uses an offline version of Draw.io by default.

## Requirements

### Microsoft Visual Studio Code

In order to install this package **Microsoft Visual Studio Code 1.51.0** at least must be installed. It is recommended to upgrade VS Code in any case.

### Python support

The new Python extensions enable VS Code as a 1st class citizen Python IDE. We recommend to use tools like `pyenv` ([here](https://github.com/pyenv/pyenv) for Linux/macOS or [here](https://github.com/pyenv-win/pyenv-win) for Windows) to install multiple Python versions and make it local to every project.

### C/C++ support

See [C/C++ for Visual Studio Code](https://code.visualstudio.com/docs/languages/cpp) for a Guide on how to configure and use the extension enabling C/C++ support for Visual Studio Code. This provides support for cross-platform C and C++ development using VS Code on Windows, Linux, and macOS.

### AsciiDoc support

AsciiDoc extension comes with Asciidoctor.js library for preview bundled. If you want to use the Ruby version of Asciidoctor you need to change the `AsciiDoc.use_asciidoctor_js` setting to false.

In order to be able to use the AsciiDoc Ruby version you have to install **Ruby** on your system and the **Asciidoctor** tool running the following command in the terminal:

```bash
gem install asciidoctor
```
