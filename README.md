## aap-cluster-build

# Introduction

This set of playbooks is designed to get past some of the initial hurdles to deploying a functional Ansible Automation Platform environment. Specifically, the playbooks do the following:

•	Download the desired AAP tarball from the Red Hat portal to the playbook directory 
•	Install package dependencies
•	Copy and extract the tarball to the automation controller that the installation will be executed from 
•	Leverage a Jinja2 template to create the inventory file that will be used in the installation
•	Run the installer script
•	Load the license manifest from the playbook directory to the automation controller

This project is by and large a development effort, and as such there are no guarantees that everything here will work without something exploding. I have put forth a best effort to add prerequisites as I come accross issues in running the setup script.