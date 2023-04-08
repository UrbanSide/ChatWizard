<p align=center>
  <img width="200" src="./assets/logo.png" alt="ChatWizard">
  <h1 align="center">ChatWizard</h1>
  <p align="center">OpenAI chat client Desktop Application (Windows, MacOS, Linux)</p>
</p>

<div align=center>
  <div align=center>
    <a href="./README-ZH_CN.md">
        <img src="https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-Simplified%20Chinese-blue" />
    </a>
  </div>
  <div>
    <img src="https://img.shields.io/github/package-json/v/lisiur/ChatWizard" />
    <img src="https://visitor-badge.glitch.me/badge?page_id=lisiur.ChatWizard" />
    <img src="https://img.shields.io/github/downloads/lisiur/ChatWizard/total" />
  </div>
  <div>
    <a href="https://github.com/lisiur/ChatWizard/releases/latest">
      <img alt="macOS" src="https://img.shields.io/badge/-macOS-black?logo=apple&logoColor=white" />
    </a>
    <a href="https://github.com/lisiur/ChatWizard/releases/latest">
      <img alt="Windows" src="https://img.shields.io/badge/-Windows-blue?logo=windows&logoColor=white" />
    </a>
    <a href="https://github.com/lisiur/ChatWizard/releases/latest">
      <img alt="Linux" src="https://img.shields.io/badge/-Linux-yellow?logo=linux&logoColor=white" />
    </a>
  </div>
</div>

## Declaration

> This project is currently undergoing active development and has only been tested on MacOS M1. In the event of any issues, please do not hesitate to submit an issue as they arise, and I will make every effort to address them. Additionally, all contributions in the form of PRs are welcome and greatly appreciated.

- All data will only be stored locally.
- Chat logs and API keys will only be used for the OpenAI API and will not be sent to any other destination.
- If concerned about API key leakage, the in-app forwarding function can be used (which enables storage of the API key on your own server, requiring only a reverse-proxy address to the OpenAI API).


## Screenshots

<details>
<summary>View</summary>
<img src="./assets/chat.jpeg" />
<img src="./assets/chat-menus.jpeg" />
<img src="./assets/chat-config.jpeg" />
<img src="./assets/prompt.jpeg" />
<img src="./assets/prompt-menus.jpeg" />
<img src="./assets/prompt-market.jpeg" />
<img src="./assets/prompt-market-menu.jpeg" />
<img src="./assets/setting.jpeg" />
<img src="./assets/light-theme.jpeg" />
</details>

## Features

- local web server
- stream response
- stop replying
- network proxy
- forward api
- lazy loading of chat records
- chat configuration
- prompt market
- local prompt
- i18n
- dark/light theme

## Todo

- [ ] multi user
- [ ] shared chat
- [ ] export pdf/image/markdown

## Installation

> If a 404 error page appears when clicking the download link, this may be due to the application being packaged at the moment. Please try again later or alternatively, download the most up-to-date version directly from [here](https://github.com/lisiur/ChatWizard/releases/latest).

- **Mac**

    - [Intel](https://github.com/lisiur/ChatWizard/releases/download/v0.0.57/ChatWizard_0.0.57_x64.dmg)
    - [Apple Silicon](https://github.com/lisiur/ChatWizard/releases/download/v0.0.57/ChatWizard_0.0.57_aarch64.dmg)

    > MacOS users may encounter this problem: `"ChatWizard.app" is damaged and can't be opened. You should move it to the Trash.`
    > 
    > open terminal and execute:
    > 
    > ```shell
    > xattr -cr /Applications/ChatWizard.app
    > ```

- **Windows**: 

    - [msi](https://github.com/lisiur/ChatWizard/releases/download/v0.0.57/ChatWizard_0.0.57_x64_en-US.msi)

- **Linux**
    - [deb](https://github.com/lisiur/ChatWizard/releases/download/v0.0.57/chat-wizard_0.0.57_amd64.deb)
    - [AppImage](https://github.com/lisiur/ChatWizard/releases/download/v0.0.57/chat-wizard_0.0.57_amd64.AppImage)

## Upgrade

ChatWizard has built-in upgrade support, and each time you restart the application, it automatically checks for any new releases. If a new version is available, a small red dot will be displayed in the lower left corner.

## Development

- dev

    ```bash
    # root
    pnpm install
    pnpm run install
    pnpm run dev
    ```

- build

    ```bash
    pnpm run build
    ```

