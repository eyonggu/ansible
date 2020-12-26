# ansible

##Inventory
Default inventory file called /etc/ansible/hosts.  You can use "-i <path>" option to specify a different inventory file.

ansible-inventory -i hosts --list

##Playbook
ansible-playbook -i hosts OptiPlex-9020.yml [-vvv]
