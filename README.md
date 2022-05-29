# microservice-deploy-ansible
Project contains docker container based application deployed in remote server using ansible.


## Prerequisites
1.  Server is ubuntu VM with ssh access using key authentication.
2.  Ansible and Python3 installed in the Client machine 



```bash
ansible-playbook -i inventory.txt --private-key=./app_server_private_key.pem main.yml
```