# buildenv
all needed for Build and Deployment done with Jenkins, ansible ....

Local enviroments for testing and dev

install Vagrant 
http://www.vagrantup.com/downloads.html

for testing Vagrantboxes
https://atlas.hashicorp.com/boxes/search?_ga=2.226081370.1915117159.1497456674-2101810526.1497456674

i like centos, so i use: 
https://atlas.hashicorp.com/centos/boxes/7

Doing Configmanagement and Bootstrap install Ansible:
http://docs.ansible.com/ansible/intro_installation.html

on mac ~/.ansible/inventory is where you define target hosts


get the host key from target system to add to knownHosts:

ssh-keyscan -H [hostname] >> ~/.ssh/known_hosts

TODO Script this

