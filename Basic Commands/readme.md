# Basic Solaris Commands

This section covers commonly used **basic Solaris administration commands**.
Each command is listed with its purpose and, where applicable, a simple example.

---

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

---

> ⚠️ Some commands may require **root or appropriate privileges** depending on system configuration.
