# Brash

## Table of Contents

- [About](#about)
- [Why Brash](#why_brash)
- [Quick Start](#quick-start)
- [Using Brash](#using-brash)
- [Examples](#examples)
- [TODO](#todo)
- [Log](#Log)
- [Help](#Help)

## About

[Brash] Cli Trash Manager full in Bash

[Brash] allows you to...

* Delete files and folders, even the ones start with "-"
* List out Trash contant
* Clean Trash
* Restore files from trash
* Nice progress viewer of what happened
* Use regular expressions

[Brash] can automatically...

* Rename existing files during Delete or Restore
* Create a trash Folder in Removable Devices

[Brash] is undergoing an interface change, please stay up to date to get the latest changes.

## Quick Start

1. Introduction:

   Installation requires :
	* [Dialog](https://invisible-island.net/dialog/) for Restore Multi select Dialog
    * [(Mawk/Gawk)](http://invisible-island.net/mawk/mawk.html) for file progress
    * [Coreutils](https://www.gnu.org/software/coreutils) for Everything else

    `Probably you just need Dialog`

2. Set up [Brash]:

	``` bash
	git clone https://github.com/zakariaGatter/brash.git ~/brash
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
  -d <FILES> : Delete File and Directories
  -c         : Clean Trash Files and Infos
  -l         : List Trash Files
  -r <FILES> : Restore Files from trash
  -s         : Trash Size
  -w <NUM>   : Wait before delete the next file in Seconds
  -v         : Explain what is being done
  -h         : Display this help text and exit

```

## Examples

* Delete file or Directory

    `brash -d EX `

    `brash -d EX*`

    `brash -d EX/*`

    `brash -d EX/[A-Z]*`

* Delete with verbose

    `brash -dv EX`

    `brash -dv EX*`

    `brash -dv EX/*`

    `brash -dv EX/[A-Z]*`

* Restore file from Trash

    `brash -r FILE_NAME`

* Restore File from Trash with dialog

    `brash -r `

* Restore File from Trash with verbose

    `brash -rv FILE_NAME`

    `brash -rv`

* Show list of files in trash

    `brash -l`

* Clean Trash

    `brash -c`

* Show Trash size

    `brash -s`

## TODO

[Brash] is a work in progress, so any ideas and patches are appreciated.

* [X] Remove Almost anything
* [X] Restore all deleted files
* [X] List all Deleted files
* [X] Clean all Trash file and info
* [X] Remove file with '-'

## LOG

* New version (31/7/2020)

    * '-w' New option
    * Make script smaller and faster
    * New and better way of get files names
    * New and better way of drive path
    * Remove the symbolic link and not the original file

## HELP

* Help needed :

    * create a man page for brash

[Brash]:http://github.com/zakariagatter/brash
