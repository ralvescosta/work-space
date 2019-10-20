# Sistema Operacional

- Linux Ubuntu 19.04

# Softwares

- ## [OH-MY-ZH](https://ohmyz.sh/)

```
sudo apt-get install zsh

sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

- ## [Visual Studio Code](https://code.visualstudio.com/docs/setup/linux)

```
sudo apt install ./<file>.deb

curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg

sudo install -o root -g root -m 644 packages.microsoft.gpg /usr/share/keyrings/

sudo sh -c 'echo "deb [arch=amd64 signed-by=/usr/share/keyrings/packages.microsoft.gpg] https://packages.microsoft.com/repos/vscode stable main" > /etc/apt/sources.list.d/vscode.list'

sudo apt-get install apt-transport-https

sudo apt-get update

sudo apt-get install code
```

- ## [NVM](https://github.com/nvm-sh/nvm)

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.0/install.sh | bash

wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.0/install.sh | bash

export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"

```

Abra o arquivo .zshrc na raiz do do HD e copie:

```
export NVM_DIR="/home/rafael/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && . "$NVM_DIR/nvm.sh"  # This loads nvm
```

- ## [Yarn](https://yarnpkg.com/en/docs/install)

- ## [Reactotron](https://github.com/infinitered/reactotron/blob/master/docs/installing.md)

- ## [Insominia](https://support.insomnia.rest/article/23-installation#ubuntu)

```
echo "deb https://dl.bintray.com/getinsomnia/Insomnia /" \
    | sudo tee -a /etc/apt/sources.list.d/insomnia.list

wget --quiet -O - https://insomnia.rest/keys/debian-public.key.asc \
    | sudo apt-key add -

sudo apt-get update

sudo apt-get install insomnia

```

- ## [Android Studio](https://developer.android.com/studio)

```
sudo add-apt-repository ppa:maarten-fonville/android-studio

sudo apt-get update

sudo apt-get install android-studio

sudo apt-get install android-studio-preview

```

- ## [Google Keep](https://keep.google.com/)

- ## [Figma-linux - snap](https://snapcraft.io/figma-linux)

```
sudo snap install figma-linux
```

- ## [DevDocs](https://github.com/freeCodeCamp/devdocs)
- ## [Spotfy](https://www.spotify.com/br/)
- ## [Slack](https://slack.com/intl/pt-br/)
- ## [Discord](https://discordapp.com/)

# Visual Studio Code Extensions

- Color Highligth
- Docker
- Dracula Official
- EditorConfig for Vs Code
- ESLint
- Material Icon Theme
- Prettier - Code formatter
- Rocketseat React Native
- Rocketseat ReactJS
- vscode-styled-components

# Environment

- ## [React Native](https://docs.rocketseat.dev/ambiente-react-native/introducao)

# Visual Studio Code - Settings.json

```json
{
  "workbench.colorTheme": "Dracula",
  "workbench.iconTheme": "material-icon-theme",
  "editor.fontSize": 18,
  "editor.lineHeight": 24,
  "editor.formatOnSave": true, //Formata antes de salvar
  "editor.rulers": [80, 120], // Margin right to limeted code
  "editor.tabSize": 2,
  "editor.renderLineHighlight": "gutter",
  "terminal.integrated.fontSize": 14,
  "emmet.syntaxProfiles": {
    "javascript": "jsx"
  },
  "emmet.includeLanguages": {
    "javascript": "javascriptreact"
  },
  "javascript.updateImportsOnFileMove.enabled": "never",
  "breadcrumbs.enabled": true,
  "editor.parameterHints.enabled": false,
  "prettier.eslintIntegration": true,
  "eslint.autoFixOnSave": true,
  "explorer.confirmDelete": false
}
```
