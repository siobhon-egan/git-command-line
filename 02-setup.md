---
title: 'Setting Up Git'
---

:::::::::::::::::::::::::::::::::::::: questions 

- How do I get set up to use Git?
- How do I configure my local machine with git? 

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Create a GitHub account
- Configure `git` the first time it is used on a computer.
- Understand the meaning of the `--global configuration` flag.

::::::::::::::::::::::::::::::::::::::::::::::::

## GitHub signup

::::::::::::::::::::::::::::::::::::: checklist

### Create account

If you have not already create a github account at https://github.com/signup

::::::::::::::::::::::::::::::::::::::::::::::::


## Local configuration

:link: [Offical GitHub documentation - setting your username](https://docs.github.com/en/get-started/getting-started-with-git/setting-your-username-in-git)

When we use Git on a new computer for the first time, we need to configure a few things. Below are a few examples of configurations we will set as we get started with Git:

- our name and email address,
- what our preferred text editor is,
- and that we want to use these settings globally (i.e. for every project).

On a command line, Git commands are written as `git verb options`, where `verb` is what we actually want to do and options is additional optional information which may be needed for the `verb.` So here is how Dracula sets up his new laptop:

Open a new terminal and configure your git workspace.

```bash
git config --global user.name "Vlad Dracula"
git config --global user.email "vlad@tran.sylvan.ia"
```

Please use your own name and email address instead of Dracula's. This user name and email will be associated with your subsequent Git activity,
which means that any changes pushed to
[GitHub](https://github.com/),
[BitBucket](https://bitbucket.org/),
[GitLab](https://gitlab.com/) or
another Git host server
after this lesson will include this information.

For this lesson, we will be interacting with [GitHub](https://github.com/) and so the email address used should be the same as the one used when setting up your GitHub account. If you are concerned about privacy, please review [GitHub's instructions for keeping your email address private][git-privacy]. 

::: callout

## Keeping your email private

If you elect to use a private email address with GitHub, then use that same email address for the `user.email` value, e.g. `username@users.noreply.github.com` replacing `username` with your GitHub one.
:::

::::::::::::::::::::::::::::::::::::::: discussion

### Line Endings

As with other keys, when you hit <kbd>Enter</kbd> or <kbd>↵</kbd> or on Macs, <kbd>Return</kbd> on your keyboard, your computer encodes this input as a character.
Different operating systems use different character(s) to represent the end of a line.
(You may also hear these referred to as newlines or line breaks.)
Because Git uses these characters to compare files, it may cause unexpected issues when editing a file on different machines. 
Though it is beyond the scope of this lesson, you can read more about this issue [in the Pro Git book](https://www.git-scm.com/book/en/v2/Customizing-Git-Git-Configuration#_core_autocrlf).

You can change the way Git recognizes and encodes line endings using the `core.autocrlf` command to `git config`. The following settings are recommended:

:::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::: solution

#### Windows

```bash
git config --global core.autocrlf true
```

:::::::::::::::::::::::::

:::::::::::::::: solution

#### MacOS and linux

```bash
git config --global core.autocrlf input
```

:::::::::::::::::::::::::

:::::::::::::::: discussion

#### Text editors

Dracula also has to set his favorite text editor, following this table:

| Editor             | Configuration command                            |
|:-------------------|:-------------------------------------------------|
| Atom | `$ git config --global core.editor "atom --wait"`|
| nano               | `$ git config --global core.editor "nano -w"`    |
| BBEdit (Mac, with command line tools) | `$ git config --global core.editor "bbedit -w"`    |
| Sublime Text (Mac) | `$ git config --global core.editor "/Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl -n -w"` |
| Sublime Text (Win, 32-bit install) | `$ git config --global core.editor "'c:/program files (x86)/sublime text 3/sublime_text.exe' -w"` |
| Sublime Text (Win, 64-bit install) | `$ git config --global core.editor "'c:/program files/sublime text 3/sublime_text.exe' -w"` |
| Notepad (Win)    | `$ git config --global core.editor "c:/Windows/System32/notepad.exe"`|
| Notepad++ (Win, 32-bit install)    | `$ git config --global core.editor "'c:/program files (x86)/Notepad++/notepad++.exe' -multiInst -notabbar -nosession -noPlugin"`|
| Notepad++ (Win, 64-bit install)    | `$ git config --global core.editor "'c:/program files/Notepad++/notepad++.exe' -multiInst -notabbar -nosession -noPlugin"`|
| Kate (Linux)       | `$ git config --global core.editor "kate"`       |
| Gedit (Linux)      | `$ git config --global core.editor "gedit --wait --new-window"`   |
| Scratch (Linux)       | `$ git config --global core.editor "scratch-text-editor"`  |
| Emacs              | `$ git config --global core.editor "emacs"`   |
| Vim                | `$ git config --global core.editor "vim"`   |
| VS Code                | `$ git config --global core.editor "code --wait"`   |

It is possible to reconfigure the text editor for Git whenever you want to change it.

:::::::::::::::: 

::::::::::::::::::::::::::::::::::::::: discussion

## Exiting text editors

Note that **Vim** is the default editor for many programs. 
If you haven’t used Vim before and wish to exit a session without saving your changes, press <kbd>Esc</kbd> then type `:q!` and hit <kbd>Return</kbd>.
If you want to save your changes and quit, press <kbd>Esc</kbd> then type `:wq` and hit <kbd>Return</kbd>.

::::::::::::::::::::::::::::::::::::::: 


## Default branch

Git (2.28+) allows configuration of the name of the branch created when you initialize any new repository. Dracula decides to use that feature to set it to main so it matches the cloud service he will eventually use.

```bash
git config --global init.defaultBranch main
```

>You can change your configuration as many times as you want: use the same commands to choose another editor or update your email address.

::::::::::::::::::::::::::::::::::::::: discussion

## Check configuration

We can check it worked by typing the following in the command line. Your username and email should appear in the output.

```bash
git config --list
```

::::::::::::::::::::::::::::::::::::::: 


::::::::::::::::::::::::::::::::::::::: challenge

## Git Help and Manual

Always remember that if you forget the subcommands or options of a `git` command, you can access the relevant list of options typing `git <command> -h` or access the corresponding Git manual by typing `git <command> --help`, e.g.:

```bash
git config -h
git config --help
```

While viewing the manual, remember the `:` is a prompt waiting for commands and you can press <kbd>Q</kbd> to exit the manual.

More generally, you can get the list of available `git` commands and further resources of the Git manual typing:

```bash
git help
```

::::::::::::::::::::::::::::::::::::::: 

:::::: callout

## One-off configuration

You only need to perform this step once per device.

::::::

---

:::::: keypoints
 - Git and GitHub are *not* the same thing. **Git** is an open source version control tool, **GitHub** is a company that hosts Git repositories in the web and provides a web interface to interact with repos they host.
 - Use `git config` with the `--global` option to configure a user name, email address, editor, and other preferences once per machine.
 - Get help with `git help`
::::::
