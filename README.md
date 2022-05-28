# microservice-deploy-ansible
Project contains docker container based application deployed in remote server using ansible.

```bash
ansible-playbook -i inventory.txt --private-key=../test-ansible_key.pem main.yml
```