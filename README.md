# To install Apache2, Jinja2, Docker, VIM, Git and Java11 in debian"

## Requirements

### Prerequisites 

To run this playbook, user needs to have Ansible installed.

For Ubuntu/Debian:
From your control node, use the following command to include PPA in your list of sources >

```bash
$ sudo apt-add-repository ppa:ansible/ansible
```
Refresh the system's package index in order to successfully add the PPA to the sources

```bash
$ sudo apt install ansible
``` 

For Fedora Workstation >

```bash
$ dnf update
$ dnf install ansible
```

### Usage

Clone the GitHub repository using the following command :

```bash
$ git clone https://github.com/skr1p7/playbook-gci.git
```

Navigate into the directory by using the following command :
```bash
$ cd playbook-gci
```

To run the playbook, use the following command 
[NOTE: The playbook is configured to be used in localhost using inventory file]

```bash
$ sudo ansible-playbook -i inventory play.yml -K
```
