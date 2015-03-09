# Cisco OpenStack Private Cloud Application Demo

This is a set of Ansible modules that will spin up a continuous
integration environment with Docker for Metacloud (now known as
Cisco OpenStack Private Cloud)

## Components

* CoreOS as the VM guest OS. 
* Docker for containers 
* Gitlab for SVN
* Jenkins for CI services (todo still)

## Prereqs

* You will need coreos bootstrap https://github.com/defunctzombie/ansible-coreos-bootstrap 

## Usage

You will need to define the following environment variables:

* OS_USERNAME="bilbo"
* OS_PASSWORD=supersecret
* OS_AUTH_URL=http://yourmetacloudidentityservice:5000/v2.0
* OS_TENANT_ID=57406d77af7643bc928cab0732ed6736
* OS_TENANT_NAME='Ring Project'

This can be easily done by navigating to the Access & Security navigation bar in Metacloud, selecting API Access and then 'Download Openstack RC file'.  This will create a file you can append to your ~/.bash_profile.


In addition you'll need to define variables that are inside the main vars/ directory.  
These are security groups and ip pools. 


