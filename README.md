# buildenv
all needed for Build and Deployment done with Jenkins, ansible ....

Local enviroments for testing and dev

## Atlas Hashicorp:

https://atlas.hashicorp.com/account/new


install Vagrant 
http://www.vagrantup.com/downloads.html

Find Boxes
https://atlas.hashicorp.com/boxes/search?_ga=2.247020429.823212900.1497608046-2101810526.1497456674

## Ansible deployments:

Doing Configmanagement and Bootstrap install Ansible:
http://docs.ansible.com/ansible/intro_installation.html

on mac ~/.ansible/inventory is where you define target hosts

example inventory:
[webservers]
192.168.33.10	ansible_ssh_user=vagrant

Test ansible runs:
ansible all -m ping

get the host key from target system to add to knownHosts:

ssh-keyscan -H [hostname] >> ~/.ssh/known_hosts

TODO Script this





