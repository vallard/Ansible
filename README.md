# Vallard's Ansible Playbooks

This is a set of ansible playbooks I am using for demo purposes. 
See my blog for more details: http://benincosa.com

The intent is to eventually show how to run Ansible with Docker on 
  * AWS
  * OpenStack (MetaCloud)
  * Digital Ocean

I also hope to add some modules for Cisco UCS, Nexus, and ACI

## Demo Setup

Do this on OSX.

```bash
brew install ansible
```

## OpenStack Demo

See the README.md file in the OpenStack Directory

## EC2 demo setup

[See my blog article for more info](http://benincosa.com/blog/?p=2651)
You'll need an AWS account.  
Add your keypair into roles/ec2/vars/main.yml so that you can log into the 
AWS instances after you create them.  

### EC2 Wordpress Demo
This demo will do the following:
  * Provision an AWS EC2 ubuntu instance (tiny-m1)
  * Install Docker and Docker Python libraries
  * Install and run a MySQL and Wordpress container  

Run the command:
```bash
cd EC2-Demo/
ansible-playbook site.yml
```
