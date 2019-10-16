# Brash

## Table of Contents

- [About](#about)
- [Why Brash](#why_brash)
- [Quick Start](#quick-start)
- [Using Brash](#using-brash)
- [TODO](#todo)

## About

[Brash] Cli Trash Manager full in Bash

[Brash] allows you to...

* Delete files and folders
* List out Trash contant
* Clean Trash
* Restore files from trash
* Nice progress viewer of what happened

[Brash] can automatically...

* Rename existing files during Delete or Restore
* Create a trash Folder in Removable Devices

[Brash] is undergoing an interface change, please stay up to date to get the latest changes.

## Quick Start

1. Introduction:

   Installation requires :
	* __Dialog__ for Restore Multi select Dialog

2. Set up [Brash]:

	``` bash
	git clone https://gitlab.com/zakariaGatter/brash.git ~/brash
	mkdir -p ~/.local/bin
	cp ~/brash/bin/brash ~/.local/bin
	chmod +x ~/.local/bin/brash
	```

## Why Brash

Well, why not. As you see its similar to [Trash_cli](https://github.com/andreafrancia/trash-cli). Unlike Trash_cli, [Brash] don't Depends on any Python libs just pure bash.

So why not ?

## Using Brash

```
BRASH Cli Trash Manager in bure Bash

brash [OPTS] [FILES]

OPTS :
  -d | --delete  : Delete File and Directories
  -c | --clean   : Clean Trash Files and Infos
  -l | --list    : List Trash Files
  -r | --restore : Restore Files from trash
  -s | --size    : Trash Size
  -v | --verbose : Verbose messages
  -h | --help    : Print help usage

NOTE :
  - File or Dirs Start with '-' can not be removed (Working on it)
```

## TODO
[Brash] is a work in progress, so any ideas and patches are appreciated.

* [X] Remove Almost anything
* [X] Restore all deleted files
* [X] List all Deleted files
* [X] Clean all Trash file and info
* [ ] Remove file with '-'


[Brash]:http://gitlab.com/zakariagatter/brash