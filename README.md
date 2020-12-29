# ansible-basics
This is repo for proof of concepts all things in here are just to play with Ansible in a basic level.


## Setup this project
```
git clone git@github.com:allexiusw/ansible-basics.git
cd ansible-basics
```

Ways in what you can create your VM are really huge, I can mention:
* Vagrant
* Docker
* Ansible with Connectors to the hypervisor
* In the virtualizer without automatization (Vmware, VirtualBox, Quemu...).

### Create VM using vagrant
```
vagrant up
```

### Run Ansible configurations
```
ansible-playbook centos8.yml --private-key=~/.ssh/id_rsa
```

And you will have the environment successfully configured.
