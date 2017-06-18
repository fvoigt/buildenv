# buildenv
all needed for Build and Deployment done with Jenkins, ansible ....

Local enviroments for testing and dev

## Atlas Hashicorp:

https://atlas.hashicorp.com/account/new


install Vagrant 
http://www.vagrantup.com/downloads.html

Find Boxes
https://atlas.hashicorp.com/boxes/search?_ga=2.247020429.823212900.1497608046-2101810526.1497456674

Me using Centos on virtual Box:
https://atlas.hashicorp.com/centos/boxes/7

Current Vagrantfile contains all tests stuff we need

# do not miss to put your public SSH Key to the VM /home/vagrant/.ssh/authorized_keys

## Ansible deployments:

Doing Configmanagement and Bootstrap install Ansible:
http://docs.ansible.com/ansible/intro_installation.html

on mac ~/.ansible/inventory is where you define target hosts

example inventory:
[build]
192.168.33.10	ansible_ssh_user=vagrant

Test ansible runs:
ansible all -m ping

perhaps disable Hostkey varification for begin:
http://docs.ansible.com/ansible/intro_getting_started.html 


### Ansible install Docker on Host  TODO: add storage handling

get Community Playbook:
ansible-galaxy install jgeusebroek.docke

cd Bootstrap
ansible-playbook ./docker.yml

### Ansible install Jenkins example

cd Bootstrap
ansible-playbook ./jenkins.yml

### Ansible install Nexus example

cd Bootstrap
ansible-playbook ./nexus.yml



