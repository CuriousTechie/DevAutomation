# DevAutomation
# In order to add new user and to grant SSH access kindly use follwoing command
ansible-playbook -i inventory/ -e "action=grant" playbooks/ssh.yml
