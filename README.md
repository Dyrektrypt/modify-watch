# Modify Watch  [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/Dyrektrypt/modify-watch/blob/master/LICENSE)
Modify Watch is a POSIX shell script for watching and controlling modified files.

## Installation
Modify Watch uses the script `mow` to actively be used in a Unix-shell; depending on the operating-system installation can vary:
> To be able to run shell script files on Windows, download and use [Git Bash](https://git-scm.com/downloads), or an alternative such as [Cygwin](https://cygwin.com/install.html).

### Step 1:
First [download](https://github.com/Dyrektrypt/modify-watch/releases/tag/1.0.0) the ZIP containing the latest Modify Watch distribution and unzip the file in your desired directory.

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
Modify Watch has the default behaviour of outputting the current date and time once a file has been modified.

Modify Watch has the following required arguments:
* `$filepath` - the path to the file to be watched