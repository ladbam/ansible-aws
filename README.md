# Ansible-AWS Installations

Base on ansible-installation file
After Installing Ansible on Master and Python on Worker

Configure SSH access on Ansible Host
# cd .ssh
# ssh-keygen
# cat id_rsa.pub

Copy the key codes from Master and paste to Worker access keys
# nano /.ssh/authorized_keys

Configure Ansible hosts file
# vi /etc/ansible/hosts
[server]
target1 ansible_ssh_host="worker IP address"

Testing Connection
# ansible all -m ping 