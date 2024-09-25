# devonfw VS Code extensions

The extensions included in this pack involve several aspects as Remote Development, Team Collaboration, Project Management, Genarative AI to assist in coding, devonfw projects development, support for other interesting languages and technologies, code running, testing, linting and IDE configuration:

> **IMPORTANT:** Please, remember to disable any of the following extensions in your workspace in case you are not allowed to use third party tools that require send code fragments to external services. More info at <https://code.visualstudio.com/docs/editor/extension-marketplace#_manage-extensions>.

- Remote Development
  - [Visual Studio Code Remote Development Extension Pack](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)
- Team Collaboration
  - [VS Live Share Extension Pack](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare-pack)
    - Please read the following instructions <https://docs.microsoft.com/en-us/visualstudio/liveshare/use/vscode>
- Project Management
  - [Project Manager](https://marketplace.visualstudio.com/items?itemName=alefragnani.project-manager)
- Gen AI

  - [Twinny](https://marketplace.visualstudio.com/items?itemName=rjmacarthy.twinny)
  
    - In order to use Twinny and run a LLM **for free and locally without external communication**, please follow the next steps:
      1. Set up Ollama as the backend by default: [Install Ollama](https://ollama.com/)
      2. Select your model from the Ollama library (e.g., `codellama:7b-instruct` for chats and `codellama:7b-code` for auto complete).
      ```bash
      $ ollama run codellama:7b-instruct
      $ ollama run codellama:7b-code
      ```
      3. Open VS Code (if already open a restart might be needed) and press Ctrl/Command + Shift + T to open the side panel. 
      
      You should see the 🤖 icon indicating that twinny is ready to use.
      
      4. See Keyboard shortcuts to start using while coding 🎉

      For other providers and other configuration alternatives, please check official [documentation](https://github.com/rjmacarthy/twinny).

- Code and documentation helpers

  - [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
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
  - [Print](https://marketplace.visualstudio.com/items?itemName=pdconsec.vscode-print)
  - [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)

- Code linting
  - [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
  - [SonarLint](https://marketplace.visualstudio.com/items?itemName=SonarSource.sonarlint-vscode)
  - Accessibility linting for HTML, Angular, React, Markdown, Vue, and React Native [axe Accessibility Linter](https://marketplace.visualstudio.com/items?itemName=deque-systems.vscode-axe-linter)
- Code runners
  - [Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner)
- JavaScript and TypeScript

  - [Angular Snippets](https://marketplace.visualstudio.com/items?itemName=johnpapa.Angular2)
  - [Angular Language Service](https://marketplace.visualstudio.com/items?itemName=Angular.ng-template)
  - [ES7 React/Redux/GraphQL/React-Native snippets](https://marketplace.visualstudio.com/items?itemName=dsznajder.es7-react-js-snippets)
  - [React Native Tools](https://marketplace.visualstudio.com/items?itemName=msjsdiag.vscode-react-native)
  - [Ionic](https://marketplace.visualstudio.com/items?itemName=ionic.ionic)
  - [Cordova Tools](https://marketplace.visualstudio.com/items?itemName=msjsdiag.cordova-tools)
  - [Jest](https://marketplace.visualstudio.com/items?itemName=Orta.vscode-jest)

    - In Linux/Mac environments and you use `nvm` as node.js version manager, if you get an error of kind `/usr/bin/env: ‘node’: No such file or directory` you can use the following setting to fix it:

    ```json
    "jest.nodeEnv": {
      "PATH": "add here your local environment path with nvm"
    },
    ```

  - [Import Cost](https://marketplace.visualstudio.com/items?itemName=wix.vscode-import-cost)
  - [Nx Console](https://marketplace.visualstudio.com/items?itemName=nrwl.angular-console) for **monorepos**. More info at <https://nx.dev/latest/angular/getting-started/console>.
  - [Pretty TypeScript Errors](https://marketplace.visualstudio.com/items?itemName=yoavbls.pretty-ts-errors)

- SCSS and CSS
  - [Stylelint](https://marketplace.visualstudio.com/items?itemName=stylelint.vscode-stylelint)
  - [SCSS IntelliSense](https://marketplace.visualstudio.com/items?itemName=mrmlnc.vscode-scss)
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
  - [rust-analyzer](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust-analyzer)
- Python
  - [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
  - [Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance)
  - [Jupyter](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)
- C++
  - [C/C++](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools)
- .NET
  - [.NET Extension Pack](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.vscode-dotnet-pack)
  - [C# Dev Kit](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csdevkit)
- Java
  - [Java Extension Pack](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack)
  - [Spring Boot Extension Pack](https://marketplace.visualstudio.com/items?itemName=Pivotal.vscode-boot-dev-pack)
  - [Community Server Connectors](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-community-server-connector)
  - [Lombok](https://marketplace.visualstudio.com/items?itemName=GabrielBB.vscode-lombok)
  - In order to make Java work properly you must set the `java.home` variable in the VS Code User Settings (Keyboard shortcut `Ctrl+,` in Windows and Linux or `Cmd+,` in macOS or press `F1` and start writing _User settings_)
  - In order to check the Java extensions for VS Code and test others available you can press F1 and choose **Java: Extension Guide**.
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
