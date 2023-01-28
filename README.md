# Ansible Playbook for Deploying Node.js Web Application

This repository contains an Ansible playbook and necessary configurations for deploying a Node.js web application on a remote server.

## Prerequisites

- A remote server with Ubuntu 18.04 or later installed, and accessible via SSH.
- Ansible 2.9 or later installed on your local machine.
- The web application package (node-ex-website-1.0.0.tgz) in the "files" directory.
- The remote server should have Node.js and npm (node package manager) installed.

## Getting Started

1. Clone the repository:

`$ git clone https://github.com/Oleh-Hudzo/ansible-node-deploy.git`

2. Change directory to the cloned repository:

`$ cd ansible-node-deploy`

3. Edit the `hosts` file to include the IP or hostname of your remote server, and the username used for SSH.
4. Edit the `project-vars` file to include the necessary variables for your deployment.
5. Run the playbook using the following command:

`$ ansible-playbook -i hosts playbooks/deploy-node.yaml`

This will run the playbook and deploy the Node.js web application on the remote server. The web application will be available on the server's IP or hostname on port 3000 by default.
You can customize the deployment process by modifying the variables in the project-vars file and re-running the playbook.

* Note: This is a sample Ansible configuration and it is intended for learning and testing purposes only. It is not production-ready and should not be used in a production environment.