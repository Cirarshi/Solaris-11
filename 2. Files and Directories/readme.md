# Files and Directories

This section covers Solaris commands used to manage files and directories.
These commands form the foundation of daily system administration and filesystem maintenance.

---

There are 3 ways of file creation using touch, mkfile, vi commands

## `touch <filename>`

Creates a empty file

**Example:**
```sh
touch f1
```

## `mkfile <size> <filename>`

Creates a file with some size

**Example:**
```sh
mkfile 2M f2
```

## `vi`

Creates a file in vi-editor mode, it will be a text file with some content.

---

## `mkdir <directory name>`

Creating a new directory


## `mkdir -p <partent directory name / child directory name / inner child directory name>`

It creates a recursive directory, like a outer one then inside it next one and so on...

**Example:**
```sh
mkdir -p one/two/three
```

## `cp <source> <destination>`

It will copy from one location to another

## `mv <source> <destination>`

It will move from one location to another
