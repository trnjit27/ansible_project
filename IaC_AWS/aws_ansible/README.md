This folder contain playbooks and files to manage AWS resources using Infrastructure as Code (IaC). The Playbook aws_playbook.yml is used to display information regarding VPCs present in region US-East-1. The AWS programmatic access has been provided using a diffenrent variables file aws_key.yml. This access variable file has been encrypted using ansible-vault. The command for the same is:

ansible-vault encrypt aws_key.yml

In order to run this playbook, needs to provide --ask-vault-pass option while running the ansible-playbook command. The command for the same is:

ansible-playbook aws_playbook.yml --ask-vault-pass
