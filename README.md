# Tauri-app

Tauri is an open-source framework that empowers developers to create native desktop applications using familiar web technologies such as HTML, CSS, and JavaScript. It presents a unique approach to application development, merging the cross-platform capabilities of web technologies with the performance and user experience advantages found in native applications (https://tauri.app). 

# Requirements

To run the application, you'll need the following:

- **NodeJS & NPM**

`Windows and macOS`: Download the Node JS installer from the official website (https://nodejs.org) and follow the installation instructions. It is recommended to download the LTS version for stability.

`Linux`: Use the package manager of your distribution to install Node JS.

```bash
sudo apt update
sudo apt install nodejs npm
```

# Pre-requisites

Before proceeding with development, you need to install the pre-requisites for developing and building tauri applications for the respective operating system.

* `Windows`: 

    * Set up the Microsoft Visual Studio C++ build tools, it's recommended to utilize the Build Tools for Visual Studio 2022 package. Build Tools for Visual Studio 2022 package: [Download Link](https://visualstudio.microsoft.com/visual-cpp-build-tools/).
    
    * Tauri relies significantly on WebView2 for rendering web content on Windows. Obtain WebView2 easily by downloading and executing the Evergreen Bootstrapper from Microsoft's official website. Evergreen Bootstrapper from Microsoft's official website: [Download Link](https://developer.microsoft.com/en-us/microsoft-edge/webview2/#download-section).
    
    * Install rust from the official rust website. Remember that you might need to restart your terminal or even your computer in some instances to ensure the changes take effect. Rust installer : [Download Link](https://www.rust-lang.org/tools/install).

* `macOS`: 

    * You will need to install CLang and macOS development dependencies. To do this, run the following command in your terminal.
    ```bash
    xcode-select --install
    ```
    
    * To install rust on macOS, open a terminal and enter the following command.
    ```bash
    curl --proto '=https' --tlsv1.2 https://sh.rustup.rs -sSf | sh
    ```
    
* `Linux`:

    * Use the package manager of your distribution to install a couple of system dependencies, such as a C compiler and webkit2gtk.
    ```bash
    sudo apt update
    sudo apt install libwebkit2gtk-4.0-dev \
    build-essential \
    curl \
    wget \
    file \
    libssl-dev \
    libgtk-3-dev \
    libayatana-appindicator3-dev \
    librsvg2-dev
    ```
    
    * To install rust on Linux, open a terminal and enter the following command.
    ```bash
    curl --proto '=https' --tlsv1.2 https://sh.rustup.rs -sSf | sh
    ```

# Running the Application

To run the application, follow these steps:

1. Clone the repository from GitHub by opening your command line or terminal and running the following command:

```bash
git clone https://github.com/OpenGenus/tauri-app
```

2. Change the current directory to the cloned repository:

```bash
cd tauri-app
```

3. Launch the application by running the command:

```bash
npm i && npm run tauri dev
```

Please note that these instructions assume you have Git installed on your system. If you don't have Git, you can also manually download the repository from GitHub by visiting the repository URL ([github.com/OpenGenus/tauri-app](https://github.com/OpenGenus/tauri-app)) and clicking on the "Code" button, then selecting "Download ZIP". After extracting the ZIP file, navigate to the extracted directory using the command line or terminal and proceed with step 3 to run the application.