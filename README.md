# ANSIBLE
## What is Ansible ?
Ansible delivers simple IT automation that ends repetitive tasks and frees up DevOps teams for more strategic work.

## This project
It contains a task to create a remote user for future administrative task with Ansible.  
As a matter of security, with this task, we don't need to allow root remote connection, and open-up sudo privileges to all users.  
Only the 'DevOps' users and groups will perform future task with Ansible.  
But to execute this, we will need to prompt the sudo password. The next configuration will be made without sudo (by changing host configuration file for the ansible master server).  
More tasks, playbooks are incoming with some app deployment: Apache, nginx, MySQL, WordPress, etc ...

## Launch the task
```console
ansible-playbook -i pre-deploy.yml
```

## More information
To understand more of ansible, we can: check it on the CLI of the master server, or on the official documentation of Ansible available [here](https://docs.ansible.com/ansible/latest/index.html)  
### Check manual on CLI
```console
ansible-doc
```
