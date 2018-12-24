# devonfw VS Code extensions

The extensions included in this pack involve several aspects as Angular, Ionic and NativeScript development, other interesting languages, code running, testing, linting and IDE configuration:

- Team Collaboration
  - [ms-vsliveshare.vsliveshare](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare)
    - Please read the following instructions https://docs.microsoft.com/en-us/visualstudio/liveshare/use/vscode
- Settings Sync
  - [Shan.code-settings-sync](https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync)
- Project Management
  - [alefragnani.project-manager](https://marketplace.visualstudio.com/items?itemName=alefragnani.project-manager)
- Code and documentation helpers
  - [christian-kohler.path-intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
  - [CoenraadS.bracket-pair-colorizer](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer)
  - [esbenp.prettier-vscode](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
    - In order to avoid TS lint errors, you must set the `prettier.singleQuote` and `prettier.semi` variables to `true` in the VS Code User Settings (Keyboard shortcut `Ctrl+,` in Windows and Linux or `Cmd+,` in macOS or press `F1` and start writing _User settings_).
    - Another useful feature to avoid TS lint errors is to set the `prettier.trailingComma` variable to `all` to trail commas wherever possible.
    - Besides this, a `.prettierrc` JSON file can be included in the root folder of any Angular project with the following configuration:
    ```json
    {
      "printWidth": 80,
      "tabWidth": 2,
      "useTabs": false,
      "semi": true,
      "singleQuote": true,
      "trailingComma": "all",
      "bracketSpacing": true,
      "arrowParens": "avoid",
      "parser": "typescript"
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
  - [joelday.docthis](https://marketplace.visualstudio.com/items?itemName=joelday.docthis)
  - [silverlakesoftware.searchdocsets-vscode](https://marketplace.visualstudio.com/items?itemName=silverlakesoftware.searchdocsets-vscode)
  - [wayou.vscode-todo-highlight](https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight)
  - [dcortes92.FreeMarker](https://marketplace.visualstudio.com/items?itemName=dcortes92.FreeMarker)
  - [pnp.polacode](https://marketplace.visualstudio.com/items?itemName=pnp.polacode)
  - [yycalm.linecount](https://marketplace.visualstudio.com/items?itemName=yycalm.linecount)
    - Please follow the instructions to configure properly this extension.
- Code runners
  - [formulahendry.code-runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner)
  - [WallabyJs.quokka-vscode](https://marketplace.visualstudio.com/items?itemName=WallabyJs.quokka-vscode)
- Angular, Ionic, NativeScript and TypeScript
  - [johnpapa.Angular2](https://marketplace.visualstudio.com/items?itemName=johnpapa.Angular2)
  - [eg2.tslint](https://marketplace.visualstudio.com/items?itemName=eg2.tslint)
  - [infinity1207.angular2-switcher](https://marketplace.visualstudio.com/items?itemName=infinity1207.angular2-switcher)
  - [jakethashi.vscode-angular2-emmet](https://marketplace.visualstudio.com/items?itemName=jakethashi.vscode-angular2-emmet)
  - [natewallace.angular2-inline](https://marketplace.visualstudio.com/items?itemName=natewallace.angular2-inline)
  - [Thavarajan.ionic2](https://marketplace.visualstudio.com/items?itemName=Thavarajan.ionic2)
  - [Telerik.nativescript](https://marketplace.visualstudio.com/items?itemName=Telerik.nativescript)
  - [vsmobile.cordova-tools](https://marketplace.visualstudio.com/items?itemName=vsmobile.cordova-tools)
  - [pnp.polacode](https://marketplace.visualstudio.com/items?itemName=pnp.polacode)
- Debuggers
  - [msjsdiag.debugger-for-chrome](https://marketplace.visualstudio.com/items?itemName=msjsdiag.debugger-for-chrome)
  - [vscjava.vscode-java-debug](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-debug)
- Git
  - [donjayamanne.githistory](https://marketplace.visualstudio.com/items?itemName=donjayamanne.githistory)
  - [eamodio.gitlens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
  - [github.vscode-pull-request-github](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github)
- Swagger and API definition
  - [Arjun.swagger-viewer](https://marketplace.visualstudio.com/items?itemName=Arjun.swagger-viewer)
- UML
  - [jebbs.plantuml](https://marketplace.visualstudio.com/items?itemName=jebbs.plantuml)
- Rust
  - [rust-lang.rust](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust)
- Python
  - [ms-python.python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
- C++
  - [ms-vscode.cpptools](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools)
- C#
  - [ms-vscode.csharp](https://marketplace.visualstudio.com/items?itemName=ms-vscode.csharp)
- Java
  - [vscjava.vscode-java-pack](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack) that will install automatically:
    - [redhat.java](https://marketplace.visualstudio.com/items?itemName=redhat.java)
    - [vscjava.vscode-java-debug](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-debug)
    - [vscjava.vscode-java-test](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-test)
    - [vscjava.vscode-maven](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-maven)
  - In order to make Java work properly you must set the `java.home` variable in the VS Code User Settings (Keyboard shortcut `Ctrl+,` in Windows and Linux or `Cmd+,` in macOS or press `F1` and start writing _User settings_)
- Key bindings
  - [ms-vscode.sublime-keybindings](https://marketplace.visualstudio.com/items?itemName=ms-vscode.sublime-keybindings)
- Docker
  - [PeterJausovec.vscode-docker](https://marketplace.visualstudio.com/items?itemName=PeterJausovec.vscode-docker)
- Themes
  - [wesbos.theme-cobalt2](https://marketplace.visualstudio.com/items?itemName=wesbos.theme-cobalt2) - Press F1, choose **Color Theme** option and select **Cobalt**.
  - [robertohuertasm.vscode-icons](https://marketplace.visualstudio.com/items?itemName=robertohuertasm.vscode-icons) - Press F1, choose **File Icon Theme** option and select **VSCode Icons**.
- Spell checking
  - [swyphcosmo.spellchecker](https://marketplace.visualstudio.com/items?itemName=swyphcosmo.spellchecker)
- AsciiDoc
  - [joaompinto.asciidoctor-vscode](https://marketplace.visualstudio.com/items?itemName=joaompinto.asciidoctor-vscode)

## Requirements

### Microsoft Visual Studio Code

In order to install this package **Microsoft Visual Studio Code 1.30.0** at least must be installed. It is recommended to upgrade VS Code in any case.

### AsciiDoc support

In order to be able to use the AsciiDoc extension you will need to install **Ruby** on your system and the **Asciidoctor** tool running the following command in the terminal:

```bash
$ gem install asciidoctor
```
