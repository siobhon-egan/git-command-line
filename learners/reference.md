---
title: Learner Reference
---

## Quick reference

### Navigating the shell

`pwd`
: print working directory

`ls`
: list directory
:
: - `-l`: list file information
: - `-lh`: list human readable file information

`cd`
: change directory


`mkdir`
: make directory

`cat`
: send file or files to output (in most cases, print to shell)

`head`
: output first parts of a file or files

`tail`
: output last parts of a file or files

`mv`
: rename or move a file or files. Syntax for renaming a file: `mv FILENAME NEWFILENAME`

`cp`
: copy a file or files. Syntax: `cp FILENAME NEWFILENAME`

`>`
: redirect output. Syntax with `cat`: `cat FILENAME1 FILENAME2 > NEWFILENAME`

`rm`
: remove a file or files. NB: *USE WITH CAUTION!!!*

### Git commands

`git init`
: create a new local git repository

`git status`
: view the status of your files in the working directory and staging area

`git add`
: tell git to start tracking a file, or a series of files

`git commit`
: save file changes from the staging area permanently to the project history

`git push`
: upload all commits to a remote repository, such as GitHub

`git log`
: show history of commits in reverse chronological order

`git diff`
: show changes made to tracked files

`git pull`
: download upstream changes and merge them into your local repository

`git remote add origin`
: add a remote repository named 'origin', to upload changes to or download changes from

## Glossary

changeset
:   A group of changes to one or more files that are or will be added
    to a single [commit](#commit) in a [version control](#version-control)
    [repository](#repository).

commit
:   To record the current state of a set of files (a [changeset](#changeset))
    in a [version control](#version-control) [repository](#repository). As a noun, 
    the result of committing, i.e. a recorded changeset in a repository.
    If a commit contains changes to multiple files,
    all of the changes are recorded together.

conflict
:   A change made by one user of a [version control system](#version-control)
    that is incompatible with changes made by other users.
    Helping users [resolve](#resolve) conflicts
    is one of version control's major tasks.

HTTP
:   The Hypertext Transfer [Protocol](#protocol) used for sharing web pages and other data
    on the World Wide Web.

merge
:   (a repository): To reconcile two sets of changes to a
    [repository](#repository).

protocol
:   A set of rules that define how one computer communicates with another.
    Common protocols on the Internet include [HTTP](#http) and [SSH](#ssh).

remote
:   (of a repository) A version control [repository](#repository) connected to another,
    in such way that both can be kept in sync exchanging [commits](#commit).

repository
:   A storage area where a [version control](#version-control) system
    stores the full history of [commits](#commit) of a project and information
    about who changed what, when.

resolve
:   To eliminate the [conflicts](#conflict) between two or more incompatible changes to a file or set of files
    being managed by a [version control](#version-control) system.

revision
:   A synonym for [commit](#commit).

SHA-1
:   [SHA-1 hashes](https://en.wikipedia.org/wiki/SHA-1) is what Git uses to compute identifiers, including for commits.
    To compute these, Git uses not only the actual change of a commit, but also its metadata (such as date, author,
    message), including the identifiers of all commits of preceding changes. This makes Git commit IDs virtually unique.
    I.e., the likelihood that two commits made independently, even of the same change, receive the same ID is exceedingly
    small.

SSH
:   The Secure Shell [protocol](#protocol) used for secure communication between computers.

timestamp
:   A record of when a particular event occurred.

version control
:   A tool for managing changes to a set of files.
    Each set of changes creates a new [commit](#commit) of the files;
    the version control system allows users to recover old commits reliably,
    and helps manage conflicting changes made by different users.
