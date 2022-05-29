# microservice-deploy-ansible
Project contains docker container based application deployed in remote server using ansible.


## Prerequisites
1. The server is an Ubuntu VM with key authentication for ssh access.
2. The client machine has Ansible and Python3 installed.
3. Admin access to the virtual machine server.

## Update dependencies

Replace and update values in file inventory.txt before running the playbook.

Update Ip Address of vm servers under [servers] section. And other arguments for groups under  [servers:vars] section

## Run Playbook
Run below command from project root directory. Replace value for file /path/to/server/private_key.pem, which is the ssh private key location

```bash
ansible-playbook -i inventory.txt --private-key=/path/to/server/private_key.pem main.yml
```

## Access Application

After successfully running the playbook application will appear in URL http://<vm_server_ip>:<port>. ie, https://3.110.166.153:3000.

Note: Make sure application port in vm server is accessaible from everywhere.

Application URL: [http://sample-application](http://3.110.166.153:3000)