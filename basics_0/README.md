
# Networking Basics #0

## Description
This project is the first in a series aimed at introducing the fundamental concepts of networking. You will learn about various networking protocols, models, and commands used to interact with and troubleshoot networks on an Ubuntu system.

## Resources
Before starting, it is recommended to read or watch the following resources:

- [OSI model](https://en.wikipedia.org/wiki/OSI_model)
- [Different types of network](https://en.wikipedia.org/wiki/Computer_network)
- [LAN network](https://en.wikipedia.org/wiki/Local_area_network)
- [WAN network](https://en.wikipedia.org/wiki/Wide_area_network)
- [Internet](https://en.wikipedia.org/wiki/Internet)
- [MAC address](https://en.wikipedia.org/wiki/MAC_address)
- [What is an IP address](https://en.wikipedia.org/wiki/IP_address)
- [Private and public address](https://en.wikipedia.org/wiki/Private_network)
- [IPv4 and IPv6](https://en.wikipedia.org/wiki/IPv6)
- [Localhost](https://en.wikipedia.org/wiki/Localhost)
- [TCP and UDP](https://en.wikipedia.org/wiki/Transmission_Control_Protocol)
- [TCP/UDP ports List](https://en.wikipedia.org/wiki/List_of_TCP_and_UDP_port_numbers)
- [What is ping / ICMP](https://en.wikipedia.org/wiki/Ping_(networking_utility))
- [Positional parameters](https://en.wikipedia.org/wiki/Parameter_(computer_programming))

### Commands to Learn (man or help):
- `netstat`
- `ping`

## Learning Objectives
By the end of this project, you should be able to explain to anyone, without the help of Google:

- **OSI Model**
  - What it is
  - How many layers it has
  - How it is organized
- **Networking Types**
  - What is a LAN: Typical usage, geographical size
  - What is a WAN: Typical usage, geographical size
  - What is the Internet
- **IP Address**
  - What it is
  - The 2 types of IP addresses
  - What is localhost
  - What is a subnet
  - Why IPv6 was created
- **TCP/UDP**
  - The two main data transfer protocols for IP (transfer level on the OSI schema)
  - The main difference between TCP and UDP
  - What is a port
  - Memorize SSH, HTTP, and HTTPS port numbers
- **Networking Tools**
  - What tool/protocol is often used to check if a device is connected to a network

## Requirements
- Allowed editors: `vi`, `vim`, `emacs`
- All your Bash script files will be interpreted on Ubuntu 20.04 LTS
- All your files should end with a new line
- A `README.md` file, at the root of the folder of the project, is mandatory
- All your Bash script files must be executable
- Your Bash script must pass Shellcheck (version 0.7.0 via `apt-get`) without any errors
- The first line of all your Bash scripts should be exactly `#!/usr/bin/env bash`
- The second line of all your Bash scripts should be a comment explaining what the script is doing

## Tasks

### 0. OSI model
- **Description:** Write answers to questions about the OSI model in a file.
- **Questions:**
  1. What is the OSI model?
  2. How is the OSI model organized?
- **File:** `0-OSI_model`
- **Directory:** `basics_0`

### 1. Types of network
- **Description:** Answer questions about different types of networks.
- **Questions:**
  1. What type of network is a computer in local connected to?
  2. What type of network could connect an office in one building to another office a few streets away?
  3. What network do you use when you browse www.google.com from your smartphone (not connected to the Wifi)?
- **File:** `1-types_of_network`
- **Directory:** `basics_0`

### 2. MAC and IP address
- **Description:** Answer questions regarding MAC and IP addresses.
- **Questions:**
  1. What is a MAC address?
  2. What is an IP address?
- **File:** `2-MAC_and_IP_address`
- **Directory:** `basics_0`

### 3. UDP and TCP
- **Description:** Fill in the blanks for TCP and UDP questions.
- **Questions:**
  1. Which statement is correct for the TCP box?
  2. Which statement is correct for the UDP box?
  3. Which statement is correct for the TCP worker?
- **File:** `3-UDP_and_TCP`
- **Directory:** `basics_0`

### 4. TCP and UDP ports
- **Description:** Write a Bash script that displays listening ports.
- **Requirements:**
  - Only shows listening sockets
  - Shows the PID and name of the program to which each socket belongs
- **File:** `4-TCP_and_UDP_ports`
- **Directory:** `basics_0`

### 5. Is the host on the network
- **Description:** Write a Bash script that pings an IP address passed as an argument.
- **Requirements:**
  - Accepts a string as an argument
  - Displays `Usage: 5-is_the_host_on_the_network {IP_ADDRESS}` if no argument passed
  - Pings the IP 5 times
- **File:** `5-is_the_host_on_the_network`
- **Directory:** `basics_0`

## Repository
- **GitHub repository:** `holbertonschool-network`
- **Directory:** `basics_0`
