# Ansible Playbooks

## Read first

Don't use any of this playbooks in production, this is just for replicate a _standard_ production host. Some of them exist just for fun :)

## Installation

* [Ansible](http://www.ansibleworks.com/docs/intro_installation.html)
* [Vagrant (testing)](http://www.vagrantup.com/downloads)

## Running it

### Vagrant

```shell
# you should have Vagrant already configured
vagrant up
```

### Ansible

```shell
# you should have Ansible already configured
ansible-playbook site.yml
```