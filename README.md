Vallard's Ansible Playbooks
===========================

This is a set of ansible playbooks I am using for demo purposes. 
See my blog for more details: http://benincosa.com

The intent is to eventually show how to run Ansible with Docker on 
  * AWS
  * OpenStack
  * Digital Ocean

I also hope to add some modules for Cisco UCS, Nexus, and ACI

Initial Setup
=============
Do this on OSX.

```bash
brew install ansible
```

[See my blog article for more info](http://benincosa.com/blog/?p=2651)

Wordpress Demo
===============
This demo will do the following:
  * Provision an AWS EC2 ubuntu instance (tiny-m1)
  * Install Docker and Docker Python libraries
  * Install and run a MySQL and Wordpress container  

Run the command:
```bash
ansible-playbook site.yml
```
