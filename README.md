# Modify Watch  [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/Dyrektrypt/modify-watch/blob/master/LICENSE)
Modify Watch is a POSIX shell script for watching and controlling modified files.

## Installation
Modify Watch uses the script `mow` to actively be used in a Unix-shell; depending on the operating-system installation can vary:
> To be able to run shell script files on Windows, download and use [Git Bash](https://git-scm.com/downloads), or an alternative such as [Cygwin](https://cygwin.com/install.html).

### Step 1:
First [download](https://github.com/Dyrektrypt/modify-watch/releases/tag/1.1.0) the ZIP containing the latest Modify Watch distribution and unzip the file in your desired directory.

### Step 2:
Open the extracted directory in terminal and run the command:

```shell
#Give the user executable permissions
chmod u+x ./mow
```

### Step 3:
Then open or create your `.bashrc` file located in the home directory (`~`) and (usually at the bottom) add, or amend:
```shell
#Make mow globally available on all terminal sessions
export PATH=$PATH:path/to/mow/directory
```

### Step 4:
Now just run the command `mow [args]` whenever you want to use Modify Watch.

## Usage
Modify Watch has the mandatory argument of SOURCE in which is the path of the file to be watched.

Modify Watch has the usage of the following:
```
Usage: mow [OPTION]... SOURCE

Output date and time of SOURCE when modified.

Mandatory arguments for long options are mandatory for short options too:
  -e, --event                  attach a shell script to be executed
  -h, --help                   bring up this help message again
  -o, --output                 attach a directory in which SOURCE will be
                               copied to
  -s, --silent                 make Modify Watch silent, giving no output
                               unless arguments are invalid

By default, Modify Watch will terminate as soon as passed files or
directories are deleted, being unable to maintain normal program flow.

Modify Watch was implemented as a more powerful alternative to
inotifywatch in which lacked essential functionality.
```