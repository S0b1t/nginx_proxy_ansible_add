#This is just a DNS config on ansible.

#First remove unnecessary lines in task files if you already have DNS settings.
#Also change th variables in the file insida vars directory.
#Don't forget to include hosts insite dns_playbook.yml file.
#Before changing variable old_date check old date with command: ansible all -m shell -a "cat /var/named/ssv.uz.db"

#Also you must be configured /etc/ansible/ansible.cfg  and /etc/ansible/hosts files.

#For instance ansible.cfg file should be:
#[defaults]
#host_key_checking = false
#inventory      = /etc/ansible/hosts

#And hosts file:
#[ubuntu]
#192.168.0.0 ansible_ssh_user=user

#After that run command ansible-playbook dns_playbook.yml
