#This is just a reverse proxy config on Apache for Ubuntu and CentOS.

#First change the variables in the file inside vars directory.
#Don't forget to include hosts insite apache_playbook.yml.

#Also you must be configured /etc/ansible/ansible.cfg  and /etc/ansible/hosts files.

#For instance ansible.cfg file should be:
#[defaults]
#host_key_checking = false
#inventory      = /etc/ansible/hosts

#And hosts file:
#[ubuntu]
#192.168.0.0 ansible_ssh_user=user

#After that run command ansible-playbook apache_playbook.yml
