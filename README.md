# Ansible-Demo
Public Repo for Demonstrating a NGINX Load Balanced Webapp Solution

Steps to Deploy this Solution from Ansible

1. Login to your Ansible control Node
2. Create a Directory using the command "mkdir Ansible_Deployment"
3. Navigate into that directory with the command "cd  Ansible_Deployment"
4. Clone the Github Repository "git clone https://github.com/GoCool2k19/Ansible-Demo.git". This will download a Folder named Ansible-Demo in your current working directory.
5. Get into the Directory Ansible-Demo/ELB "cd Ansible-Demo/ELB/group_vars/"
6. Open up the variables file named "all" in Vi editor "vi all", copy all the contents in a notepad and close the file.
7. Delete the file named all. "rm all"
8. In your notepad, replace the xxxxxxxxxx with apt values for ec2_access_key and ec2_secret_key.(These are AWS IAM User Credentials with which we are going to perform resource spawning/managing from Ansible playbooks remotely from Ansible Control Node) 
9. From the Ansible Control Node server, create an Ansible Vault to encrypt and store these AWS secrets/credentials and Ansible variables.
