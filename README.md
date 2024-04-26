# Ansible Playbook Examples

## Description
This playbook is intended to provide useful samples of common system administration tasks in playbooks for both Linux and Windows. In a production playbook, we would make more use of advanced ansible features like roles to promate reusability and do things like make more use of loops, and variables ot make the playbook easier to maintain.

These are good playbooks to practice and try to get working in a test environment. As you start to scale and grow in your approach you will want a tool to help orchestrate and manage playbook runs. There are excellent Open-Source and Paid solutions depending on your needs for support and your environment. I would recommend either Semaphore or Ansible Automation.

## Dev Container
This repository includes a fedora dev container built for Ansible playbook development. To use the dev container, install Docker Desktop, visual studio code, and the dev-containers VSCode extension. Click the connection icon near the bottom left of VSCode and select open in Container.

## Ansible Vault
Replace the encrypted secret files with your own and use ansible vault to encrypt and decrypt. For more info on using ansible vault, go here.
https://www.redhat.com/sysadmin/ansible-playbooks-secrets

## Usage
### Windows Playbook
ansible-playbook playbook-windows.yml -i development.yml --ask-pass --ask-vault-pass

### Linux Playbook
ansible-playbook playbook-linux.yml -i development.yml --ask-pass --ask-become-pass --ask-vault-pass

## References
I want to send a huge thank you to some of the blog posts that helped me pull all of this together.
https://serverspike.io/automating-active-directory-authentication-on-linux-with-ansible/
https://www.redhat.com/sysadmin/ansible-playbooks-secrets
https://4sysops.com/archives/install-ansible-on-windows/#:~:text=Install%20Ansible%20on%20Windows%201%20Install%20Ansible%20Once,inventory%20file%20...%204%20Enable%20PowerShell%20remoting%20

