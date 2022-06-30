# Remote Control Using Ansible

This playbook automates the configuration of an ec2 instance by adapating manual instructions to ansible playbook tasks.

## Prerequisites
1. Key pair: You should have an AWS EC2 key pair already created in your AWS Console, and downloaded to your local machine.
2. EC2 instance: An AWS EC2 Ubuntu instance mapped with the udacity.pem key-pair should be running in your AWS account
3. Inventory file: The inventory file containing the public IP address of your AWS EC2 Ubuntu VM must be present in your exercise directory.
`[all]
\#Your ec2 instance public ip address here`

Run using `ansible-playbook -i your_inventory_file main.yml -- private-key your_private_key_location`