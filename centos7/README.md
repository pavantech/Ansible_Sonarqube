Ansible is an IT automation tool. It can configure systems, deploy software, and orchestrate more advanced IT tasks such as continuous deployments or zero downtime rolling updates.
First you need to install ansible on centos. 
Steps for Redhat Family: 
# wget http://dl.fedoraproject.org/pub/epel/7/x86_64/e/epel-release-7-9.noarch.rpm
# rpm -ivh epel-release-7-9.noarch.rpm
# yum install ansible
# ansible --version
# sudo yum install git
Steps for debain Family:
# sudo apt-get update
# sudo apt-get install software-properties-common
# sudo apt-add-repository ppa:ansible/ansible
# sudo apt-get update
# sudo apt-get install ansible
# sudo apt-get install git

Steps to run this code:
git clone https://github.com/pavantech/Ansible_jenkins.git
cd Ansible_jenkins
vi hosts
[jenkins] 
xx.xx.xx ansible_ssh_user=username ansible_ssh_pass=password 

Save esc:wq

You need to add the username and password of target server in this hosts file.

This code witten based on target server of Redhat family. 

# ansible-playbook main.yml








