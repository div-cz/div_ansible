# div_ansible
Make a server great again.

## Table of Contents
1. [Prerequisites](#prerequisites)
2. [How to start](#how-to-start)
3. [Local Computer](#local-computer)
4. [Server 1](#server-again)
5. [License](#license)

## Prerequisites<!--#prerequisites-->
Ubuntu server 23.10

## How to start<!--#how-to-start-->
- sudo apt update
- sudo apt upgrade
- sudo apt install ansible
- cd /home/user/.ansible
- touch hosts
- nano hosts
    - webservers: 
    - 46.28.110.160
- touch ansible.cfg
    - [defaults]
    - inventory = /home/divcz/.ansible/hosts
    - host_key_checking = False
    - remote_user = divcz
    - private_key_file=/home/divcz/.ssh/ansible_rsa
    - [ssh_connection]
    - ssh_args = -o ServerAliveInterval=10

## Local computer<!--#local-computer-->
- cd /tmp
- git clone https://github.com/div-cz/div_ansible.git
- RUN PowerShell as an administrator
    - wsl --install

## License<!--#license-->
This project is shared under the MIT License. See `LICENSE.md` for details.
