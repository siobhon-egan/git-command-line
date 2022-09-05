---
title: Setup
---

# :computer: **Software requirements**

## Bash

::::::::::::::::::::::::::::::::::::::: discussion

### Details

The shell is a program where users can type commands. 
The most popular Unix shell is **Bash** (the Bourne Again SHell — so-called because it’s derived from a shell written by Stephen Bourne). 
Bash is the default shell on most modern implementations of Unix and in most packages that provide Unix-like tools for Windows.

Some computers include a default Unix Shell program. 
The steps below describe some methods for identifying and opening a Unix Shell program if you already have one installed. There are also options for identifying and downloading a Unix Shell program, a Linux/UNIX emulator, or a program to access a Unix Shell on a server.

:::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::: solution

### Windows

Computers with Windows operating systems do not automatically have a Unix Shell program installed. In this lesson, we encourage you to use an emulator included in [Git for Windows](https://carpentries.github.io/workshop-template/#shell), which gives you access to both Bash shell commands and Git.

- **1.** Download the Git for Windows [installer](https://gitforwindows.org/).
- **2.** Run the installer and follow the steps below:
    - 2.1. Click on "Next" four times (two times if you've previously installed Git). You don't need to change anything in the Information, location, components, and start menu screens.
    - 2.2. **From the dropdown menu, "Choosing the default editor used by Git", select "Use the Nano editor by default" (NOTE: you will need to scroll up to find it) and click on "Next".**
    - 2.3. On the page that says "Adjusting the name of the initial branch in new repositories", ensure that "Let Git decide" is selected. This will ensure the highest level of compatibility for our lessons.
    - 2.4. Ensure that "Git from the command line and also from 3rd-party software" is selected and click on "Next". (If you don't do this Git Bash will not work properly, requiring you to remove the Git Bash installation, re-run the installer and to select the "Git from the command line and also from 3rd-party software" option.)
    - 2.5. Select "Use bundled OpenSSH".
    - 2.6. Ensure that "Use the native Windows Secure Channel Library" is selected and click on "Next".
    - 2.7. Ensure that "Checkout Windows-style, commit Unix-style line endings" is selected and click on "Next".
    - 2.8. **Ensure that "Use Windows' default console window" is selected and click on "Next".**
    - 2.9. Ensure that "Default (fast-forward or merge) is selected and click "Next"
    - 2.10. Ensure that "Git Credential Manager" is selected and click on "Next".
    - 2.11. Ensure that "Enable file system caching" is selected and click on "Next".
    - 2.12. Click on "Install".
    - 2.13. Click on "Finish" or "Next".

- **3.** If your "HOME" environment variable is not set (or you don't know what this is):
    - 3.1. Open command prompt (Open Start Menu then type `cmd` and press <kbd>Enter</kbd>)
    - 3.2. Type the following line into the command prompt window exactly as shown: `setx HOME "%USERPROFILE%"`
    - 3.3. Press <kbd>Enter</kbd>, you should see `SUCCESS: Specified value was saved.`
    - 3.4. Quit command prompt by typing `exit` then pressing <kbd>Enter</kbd>.

[Check out video tutorial here](https://youtu.be/339AEqk9c-8)

Once installed, you can open a terminal by running the program **Git Bash** from the Windows start menu.

:::::::::::::::::::::::::

:::::::::::::::: solution

### MacOS

For a Mac computer running macOS Mojave or earlier releases, the default Unix Shell is Bash. For a Mac computer running macOS Catalina or later releases, the default Unix Shell is Zsh. Your default shell is available via the Terminal program within your `/Applications/Utilities` folder.

To open Terminal, try one or both of the following:

- In Finder, select the Go menu, then select Utilities. Locate Terminal in the Utilities folder and open it.
- Use the Mac ‘Spotlight’ computer search function. Search for: `Terminal` and press <kbd>Return</kbd>.

See the Git installation [video tutorial](https://carpentries.github.io/workshop-template/#shell-macos-video-tutorial) for an example on how to open the Terminal. You may want to keep Terminal in your dock for this workshop.

To check if your machine is set up to use something other than Bash, type `echo $SHELL` in Terminal and press the <kbd>Return</kbd> key.

If your machine is set up to use something other than Bash, you can run it by opening a terminal and typing `bash`.

If you want to change your default shell, see this [Apple Support article](https://support.apple.com/en-au/HT208050) and follow the instructions on "How to change your default shell".

[Check out video tutorial here](http://www.youtube.com/watch?v=9LQhwETCdwY)

:::::::::::::::::::::::::

:::::::::::::::: solution

### Linux

The default shell is usually Bash and there is usually no need to install anything.

To see if your default shell is Bash type `echo $SHELL` in a terminal and press the <kbd>Enter</kbd> key. If the message printed does not end with '/bash' then your default is something else and you can run Bash by typing `bash`.

:::::::::::::::::::::::::

## Git

::::::::::::::::::::::::::::::::::::::: discussion

### Details

Git is a version control system that lets you track who made changes to what when and has options for easily updating a shared or public version of your code on [github.com](https://github.com/). You will need a [supported web browser](https://help.github.com/articles/supported-browsers/).

You will need an account at [github.com](https://github.com/) for parts of the Git lesson. Basic GitHub accounts are free. We encourage you to create a GitHub account if you don't have one already. Please consider what personal information you'd like to reveal. For example, you may want to review these [instructions for keeping your email address private](https://help.github.com/articles/keeping-your-email-address-private/) provided at GitHub.

:::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::: solution

### Windows

Git should be installed on your computer as part of your Bash install (see the [Shell installation instructions](https://carpentries.github.io/workshop-template/#shell)).

You can check by opening the program **Git Bash** and entering `git`.

If you see this error, then you should try to install git again. 

```error
'git' is not recognised as an internal or external command,
operable program or batch file.
```

:::::::::::::::::::::::::

:::::::::::::::: solution

### MacOS

**For macOS**, install Git for Mac by downloading and running the most recent "mavericks" installer from [this list](http://sourceforge.net/projects/git-osx-installer/files/). Because this installer is not signed by the developer, you may have to right click (control click) on the .pkg file, click Open, and click Open on the pop up window. After installing Git, there will not be anything in your `/Applications` folder, as Git is a command line program. **For older versions of OS X (10.5-10.8)** use the most recent available installer labelled "snow-leopard" [available here](http://sourceforge.net/projects/git-osx-installer/files/).

You can check your version of git by opening **Terminal** and entering `git --version`.
```output
git version 2.24.3 (Apple Git-128)
```

[Check out video tutorial here](https://youtu.be/9LQhwETCdwY)

:::::::::::::::::::::::::

:::::::::::::::: solution

### Linux

If Git is not already available on your machine you can try to install it via your distro's package manager. For Debian/Ubuntu run `sudo apt-get install git` and for Fedora run `sudo dnf install git`.

:::::::::::::::::::::::::

## Text editor

::::::::::::::::::::::::::::::::::::::: discussion

### Details

When you're writing code, it's nice to have a text editor that is optimized for writing code, with features like automatic color-coding of key words. 

_**Exiting common text editors**_

The default text editor on macOS and Linux is usually set to **Vim**, which is not famous for being intuitive. If you accidentally find yourself stuck in it, hit the <kbd>Esc</kbd> key, followed by <kbd>:</kbd> + <kbd>Q</kbd> + <kbd>!</kbd> (colon, lower-case 'q', exclamation mark), then hitting <kbd>Return</kbd> to return to the shell.
To exit **nano** text editor (which is recommended during later lessons) press <kbd>Control</kbd> + <kbd>X</kbd>, it will prompt you to save changes press <kbd>Y</kbd> and <kbd>Return</kbd>.

:::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::: solution

### Windows

nano is a basic editor and the default that instructors use in the workshop. It is installed along with Git.

:::::::::::::::::::::::::

:::::::::::::::: solution

### MacOS

nano is a basic editor and the default that instructors use in the workshop. See the Git installation video tutorial for an example on how to open nano. It should be pre-installed.

[Check out video tutorial here](https://youtu.be/9LQhwETCdwY)

:::::::::::::::::::::::::

:::::::::::::::: solution

### Linux

nano is a basic editor and the default that instructors use in the workshop. It should be pre-installed.

:::::::::::::::::::::::::
