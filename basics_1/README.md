
# Networking Basics #1

## Description
This project is part of a series on networking basics. You will learn how to configure and manipulate various aspects of networking on an Ubuntu machine. You will use different tools and commands to display and configure network interfaces, as well as test network connections.

## Resources
Before starting, it is recommended to read or watch the following resources:

- [What is localhost](https://www.computerhope.com/jargon/l/localhost.htm)
- [What is 0.0.0.0](https://en.wikipedia.org/wiki/0.0.0.0)
- [What is the hosts file](https://www.howtogeek.com/howto/27350/beginner-geek-how-to-edit-your-hosts-file/)
- [Netcat examples](https://www.digitalocean.com/community/tutorials/how-to-use-netcat-to-establish-and-test-tcp-and-udp-connections)
- Commands to consult with `man` or `help`: `ifconfig`, `telnet`, `nc`, `cut`

## Learning Objectives
By the end of this project, you should be able to explain to anyone, without the help of Google:

- What is `localhost`/`127.0.0.1`
- What is `0.0.0.0`
- What is `/etc/hosts`
- How to display your machine’s active network interfaces

## Requirements
- Allowed editors: `vi`, `vim`, `emacs`
- All your files will be interpreted on Ubuntu 20.04 LTS
- All your files should end with a new line
- A `README.md` file, at the root of the folder of the project, is mandatory
- All your Bash script files must be executable
- Your Bash script must pass `Shellcheck` (version 0.7.0 via `apt-get`) without any errors
- The first line of all your Bash scripts should be exactly `#!/usr/bin/env bash`
- The second line of all your Bash scripts should be a comment explaining what the script is doing

## Tasks

### 0. Change your home IP
- **Description:** Write a Bash script that configures an Ubuntu server with the following requirements:
  - `localhost` resolves to `127.0.0.2`
  - `facebook.com` resolves to `8.8.8.8`
- **File:** `0-change_your_home_IP`
- **Example:**
  ```bash
  sylvain@ubuntu$ sudo ./0-change_your_home_IP
  sylvain@ubuntu$ ping localhost
  PING localhost (127.0.0.2) 56(84) bytes of data.
  64 bytes from localhost (127.0.0.2): icmp_seq=1 ttl=64 time=0.012 ms
  ```

### 1. Show attached IPs
- **Description:** Write a Bash script that displays all active IPv4 IPs on the machine.
- **File:** `1-show_attached_IPs`
- **Example:**
  ```bash
  sylvain@ubuntu$ ./1-show_attached_IPs | cat -e
  10.0.2.15$
  127.0.0.1$
  ```

### 2. Port listening on localhost
- **Description:** Write a Bash script that listens on port 98 on localhost.
- **File:** `2-port_listening_on_localhost`
- **Example:**
  ```bash
  Terminal 0
  sylvain@ubuntu$ sudo ./2-port_listening_on_localhost

  Terminal 1
  sylvain@ubuntu$ telnet localhost 98
  Trying 127.0.0.2...
  Connected to localhost.
  Escape character is '^]'.
  Hello world
  test
  ```

## Notes
- Before running these scripts on a machine you will continue to use, make sure to revert `localhost` to `127.0.0.1`. Otherwise, many things might stop working.

## Repository
- **GitHub repository:** `holbertonschool-network`
- **Directory:** `basics_1`

