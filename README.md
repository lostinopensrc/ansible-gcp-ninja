# OVERVIEW

This repository is a POC for deploying GCP resources using Ansible Google Cloud Collections named : google.cloud 

This collection is not a part of ansible-core and needs to be install seperately using command :

ansible-galaxy collection install google.cloud

To perform installtion of collection we have a Ansible Playbook and a github action Workflow as shown in below image:

![Pre-requistes](images/pre-requistes.JPG)


## GITHUB REPO Structure :

![Repo-Structure](images/Repo_Structure.JPG)

As per above image this repo makes use of Ansible group_vars concept and the structure is divided as follows:

1. Github Workflows: Each GCP resource creation has a github action workflow Job.
2. Each GCP resource being made has there own vars.yaml file under group_vars/resource directory.
3. playbooks directory contains ansible playbooks for creation of each resource.


## High level Flow Diagram :

![HLD](images/Ansible_IAC_GCP.JPG)