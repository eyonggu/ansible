# ansible

##installing Ansible on Ubuntu
'''
sudo apt update
sudo apt install software-properties-common
sudo apt-add-repository --yes --update ppa:ansible/ansible
sudo apt install ansible
'''

##Inventory
Default inventory file called /etc/ansible/hosts.  You can use "-i <path>" option to specify a different inventory file.

ansible-inventory -i hosts --list

##Playbook
ansible-playbook playbooks/Ubuntu.yml -i hosts [-vvv]
ansible-playbook playbooks/Ubuntu.yml -i hosts --limit "<host>"

###Check for syntax
ansible-playbook playbooks/Ubuntu.yml --syntax-check

###Dry-run a playbook
ansible-playbook playbooks/Ubuntu.yml --check
