# Basic Solaris Commands

This section covers commonly used **basic Solaris administration commands**.
Each command is listed with its purpose and, where applicable, a simple example.

---

## `bash`

Activate user friendly session

## `date`

Display current date and time with time zone

## `cal`

Display current month calender

**Example:**
```sh
cal 8 2025
```
## `bc`

Activate binary calculator

## `pwd`

Display present working directory

## `cd`

It is for changing directories

**Example:**
```sh
cd ..
```

## `uname`

Dispalys name of the OS

**Example:**
```sh
uname -a
```
display the name, platform and all other details

## `top`

Displays real-time information about system processes and resource usage such as CPU and memory.

- Refreshes automatically every **5 seconds**
- Useful for monitoring system load and identifying resource-heavy processes

**Example:**
```sh
top
```

---

## `which <command>`

Displays the full path of the specified command executable.

- Helps verify which binary is being executed
- Useful when multiple versions of a command exist in the system

**Example:**
```sh
which ls
```

---

## `hostname`

Displays or sets the system hostname.

- Without arguments, it shows the current hostname
- With an argument, it changes the hostname (temporary until reboot unless configured permanently)

**Example:**
```sh
hostname
```

Set hostname to `UK`:
```sh
hostname UK
```

---

## `uptime`

Displays how long the system has been running along with the load average and number of logged-in users.

- Helpful for checking system stability and load trends

**Example:**
```sh
uptime
```

## `whoami`

Display the current user

## `hostid`

Displays host id of current user

## `man <command>`

Display the details of the command

**Example:**
```sh
man cd
```

---

**Example:**
```sh
top | wc -l
```
The above one counts the number of lines of output of a command

---

> ⚠️ Some commands may require **root or appropriate privileges** depending on system configuration.
