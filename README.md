# Ansible Playbooks

## Read first

Don't use any of this playbooks in production, this is just for replicating a _standard_ production host. Some of them exist just for fun :)

## Ansible
### Python + ssh = happiness

> Ansible is a radically simple configuration-management, deployment, task-execution, and multinode orchestration framework.

* [Documentation](http://docs.ansible.com/)

### Installation

* [Homebrew](http://brew.sh/)
* [Ansible](http://devopsu.com/guides/ansible-ubuntu-debian.html)
* [Python on OS X](http://docs.python-guide.org/en/latest/starting/install/osx/)
* [Disabling root for user](http://stackoverflow.com/questions/14926562/activating-the-root-user-with-a-python-script-osx)

> AnsibleWorks Galaxy is your hub for finding, reusing, and sharing the best Ansible content.

Ansible + Galaxy =~ Rubygem|pip|…

* [Documentation](https://galaxy.ansibleworks.com/)

### Galaxy roles

* [MySQL](https://galaxy.ansibleworks.com/list#/roles/1)

### Using galaxy

```yml
- hosts: all
  roles:
  - {role: role_name, role_var1: foobar, role_var2: none, role_var3: none }
```

## Vagrant
### Dirty testing

Virtual machine + Ruby = ....

![webscale-everywhere](http://what-if.xkcd.com/imgs/a/20/diamond_11.png)

* [Documentation](http://docs.vagrantup.com/v2/)

To quickly run some playbook on a fresh vagrant I use a `Rakefile`, there is a sample [here](https://github.com/Awea/ansible-playbooks/blob/master/sample.Rakefile).

```ruby
# run it !
rake test
```

### vre alias
#### zsh ftw !

```shell
# Vagrant aliases
alias vdf="vagrant destroy -f"
alias vup="vagrant up"
alias vre="vdf && vup"
```

## Sites
### site.yml
Run Mumble.

### default.site.yml
Runs nginx, Transmission and its web interface.
