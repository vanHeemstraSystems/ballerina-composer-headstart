# 100 Visual Studio Code Plugin

Start with having Visual Studio Code installed on your server (here CentOS 7).

## How to Install Visual Studio Code on CentOS 7

Source: https://linuxize.com/post/how-to-install-visual-studio-code-on-centos-7/

[Visual Studio Code](https://code.visualstudio.com/) is an open-source cross-platform code editor developed by Microsoft. It has a built-in debugging support, embedded [Git](https://linuxize.com/post/how-to-install-git-on-centos-7/) control, syntax highlighting, code completion, integrated terminal, code refactoring and snippets.

The easiest and recommended way to install Visual Studio Code on CentOS machines is to enable the VS Code repository and install the VS Code package through the command line.

### Prerequisites

You’ll need to be logged in as a ***user with sudo access*** to be able to install packages.

### Installing Visual Studio Code on CentOS

Perform the following steps to install Visual Studio Code on your CentOS system:

#### 01. Start by importing the Microsoft GPG key:

```$ sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc```

#### 02. Next, create the following repo file to enable the Visual Studio Code repository:

```$ sudo nano /etc/yum.repos.d/vscode.repo```

Paste the following content into the file:

```
[code]
name=Visual Studio Code
baseurl=https://packages.microsoft.com/yumrepos/vscode
enabled=1
gpgcheck=1
gpgkey=https://packages.microsoft.com/keys/microsoft.asc
```
/etc/yum.repos.d/vscode.repo

#### 03. Once the repository is enabled, install the latest version of Visual Studio Code by typing:

```$ sudo yum install code```

That’s it. Visual Studio Code has been installed on your CentOS desktop and you can start using it.

## Starting Visual Studio Code

Now that VS Code is installed on your CentOS system you can launch it either from the command line by typing ```code``` or by clicking on the VS Code icon (Applications -> Programming -> Visual Studio Code).

When you start VS Code for the first time, a window should appear.

You can now start installing extensions and configuring VS Code according to your preferences.

## Updating Visual Studio Code

When a new version is released you can update the Visual Studio Code package through your desktop standard Software Update tool or by running the following command in your terminal:

```$ sudo yum update```

## Conclusion

You have successfully installed VS Code on your CentOS 7 machine. To learn more about VS Code visit their official [documentation](https://code.visualstudio.com/docs/) page.

## Installing the Ballerina Composer Plugin

...
