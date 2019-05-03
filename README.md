# DevAutomation #Instuctions to run commnads
1)In order to add new user and to grant SSH access kindly use the command:
ansible-playbook -i inventory/ -e "action=grant" playbooks/ssh.yml

2)In order to grant ssh access to an existing user kindly use the command: 
ansible-playbook -i inventory/ -e "action=grant" playbooks/ssh.yml --skip-tags=add

3)In order to revoke ssh access from user.Kindly use the command: 
ansible-playbook -i inventory/ -e "action=revoke" playbooks/ssh.yml --skip-tags=remove

4)In order to remove use kindly use the command:
ansible-playbook -i inventory/ -e "action=revoke" playbooks/ssh.yml

