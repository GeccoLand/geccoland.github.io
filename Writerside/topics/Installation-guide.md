---
switcher-label: Installation
---

# Gecco Installation Guide
<show-structure for="none"/>

> Use the switcher in the top bar to select the guide for your specific operating system.

This guide provides step-by-step instructions to install Gecco on Windows, Linux, and macOS. Whether you're a seasoned
developer or new to programming, follow the appropriate section to set up Gecco on your system quickly.

<!-- 
##########################################
WINDOWS SECTION START
##########################################
-->

## Windows System Requirements {switcher-key="Windows"}

Before you begin, ensure your system meets the following minimum requirements:

- Operating System: Windows 10 or later
- RAM: 4 GB or more
- Disk Space: 500 MB free space
- Compiler: Dependencies: GCC 10+

## **Installation on Windows** {switcher-key="Windows"}

1. **Download Gecco Installer:**
    - Visit the official Gecco [website](https://gecco.dev/download)
    - Navigate to the Windows section and select the Windows Installer.
2. **Run the Installer:**
    - Double-click the installer file (`GeccoSetup.exe`).
    - Follow the on-screen instructions to complete the installation.
3. **Set Environment Variables:**
    - During installation, the installer should add Gecco to your system’s PATH. If not:
    - Go to **Control Panel > System > Advanced System Settings**.
    - Click **Environment Variables** and add the Gecco installation directory (e.g., `C:\Gecco`) to the PATH variable.
4. **Verify Installation:**
    - Open Command Prompt and run:
       ```console
       gecco --version
       ```
    - You should see the installed version of Gecco.

## **Updating Gecco on Windows** {switcher-key="Windows"}

To update to the latest version of Gecco:

- Download the latest installer and follow the installation steps.

## **Uninstallation on Windows** {switcher-key="Windows"}

- Use the Add/Remove Programs feature in the Control Panel to uninstall Gecco.

<!-- 
##########################################
WINDOWS SECTION END
##########################################
-->

<!-- 
##########################################
MACOS SECTION START
##########################################
-->

## macOS System Requirements {switcher-key="macOS"}

Before you begin, ensure your system meets the following minimum requirements:

- Operating System: macOS 10.15 (Catalina) or later
- RAM: 4 GB or more
- Disk Space: 500 MB free space
- Compiler: Dependencies: Clang 11+

## **Installation on macOS** {switcher-key="macOS"}

### Using Homebrew (Recommended)

   1. **Install Homebrew (if not already installed):**
    - Run the following command in Terminal:
        ```bash
        /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
        ```
   2. **Add the Gecco Formula**
       - Add the official Gecco tap:
        ```bash
         brew tap gecco/tap
        ```
   3. **Install Gecco**
       - Run:
         ```Bash
         brew install gecco
         ```
   4. **Verify the Installation**
      - Open Terminal and run:
         ```bash
         gecco --version 
        ```
### From Source
   1. **Download the Source Code**
      - Clone the repository:
         ```bash
        git clone https://github.com/GeccoLand/Gecco.git
        cd gecco
        ```
   2. **Install Dependencies**
      - Ensure Xcode command-line tools are installed:
         ```bash
         xcode-select --install 
        ```
   3. **Build Gecco**
      - Run the build script:
         ```bash
        ./build.sh 
        ```
   4. **Install Gecco**
      - Install the built binaries:
        ```Bash
        sudo ./install.sh
        ```
   5. **Verify the Installation**
      - Run:
         ```bash
         gecco --version
         ```

### **Updating Gecco on macOS**
- Pull the latest changes from the repository and reinstall:
  ```bash
  cd gecco
  git pull origin main
  ./install.sh
  ```

### **Uninstallation on macOS**
- Remove the Gecco binary and related files:
  ```bash
  sudo rm -rf /usr/local/bin/gecco
  sudo rm -rf /usr/local/lib/gecco
  ```

<!-- 
##########################################
MACOS SECTION END
##########################################
-->

<!-- 
##########################################
LINUX SECTION START
##########################################
-->

## Linux System Requirements {switcher-key="Linux"}

Before you begin, ensure your system meets the following minimum requirements:

- Operating System: Linux distribution with a 64-bit kernel.
- RAM: 4 GB or more
- Disk Space: 500 MB free space
- Compiler: Clang 11+

## **Installation on Linux** {switcher-key="Linux"}

### Using Package Manager (Recommended)

1. **Add the Gecco Repository**
    - For Debian-based systems(e.g., Ubuntu):
      ```bash
      sudo add-apt-repository ppa:gecco/stable
      sudo apt update
      ```
    - For RPM-based systems (e.g., Fedora):
      ```bash
      sudo dnf config-manager --add-repo https://gecco.dev/repo/gecco.repo
      sudo dnf update
      ```
2. **Install Gecco**
    - On Debian-based systems
      ```bash
      sudo apt install gecco
      ```
    - On RPM-based systems:
      ```Bash
      sudo dnf install gecco
      ```
3. **Verify the Installation**
    - Open a terminal and run:
      ```Bash
      gecco --version
      ```
    - The installed version of Gecco should be displayed.

### From the Source Code

1. **Download the Source Code**
    - Clone the Gecco repository:
      ```bash
      git clone https://github.com/GeccoLand/Gecco.git
      cd gecco
      ```

2. **Build Gecco**
    - Ensure you have Clang installed:
      ```bash
      sudo apt install build-essential
      ```
    - Run the build script:
      ```Bash
      ./build.sh
      ```
3. **Install Gecco**
    - Install the built binaries:
      ```bash
      sudo ./install.sh
      ```
4. **Verify the Installation**
    - Run:
      ```bash
      gecco --version
      ```

### **Updating Gecco on Linux**
   - Pull the latest changes from the repository and reinstall:
      ```bash
      cd gecco
      git pull origin main
      ./install.sh
      ```

### **Uninstallation on Linux**
   - Remove the Gecco binary and related files:
      ```bash
      sudo rm -rf /usr/local/bin/gecco
      sudo rm -rf /usr/local/lib/gecco
      ```

<!-- 
##########################################
LINUX SECTION END
##########################################
-->
---

For additional help, visit the [Gecco Support Center](https://gecco.dev/support) or join our community forums.


