# Installing Dotfiles for Remote Server via Ansible
## Description
This Ansible playbook is basically adding the ubuntu ppa for [Fish Shell v3](https://fishshell.com/) and then installing [Fish Shell v3](https://fishshell.com/). For [Fish Shell v3](https://fishshell.com/) we also install [Starship](https://starship.rs/) as our prompt and then apply a [custom config](https://github.com/TimyStream/dotfiles/tree/remoteServer) that i made for Remote Server.
## How to use
create a Python virtual environment called "venv" like this:
`python3 -m venv venv`

Based on you shell activate it with:
- Bash
    - `source ./venv/bin/activate`
- Fish
    - `source ./venv/bin/activate.fish`

after this you just need to install [Ansible](https://www.ansible.com/) with
`pip install ansible==6.7.0`

now all you have to do is replace "exampleHost" in the inventory with the your hostIP or domain name! Don't forget to also change the "ansible_user" and the "ansible_become_pass" to the right values.