# ansible-setup on ubuntu
## all command
sudo su

# From your control node, run the following command to include the official project’s PPA (personal package archive) in your system’s list of sources:
sudo apt-add-repository ppa:ansible/ansible

# Next, refresh your system’s package index so that it is aware of the packages available in the newly included PPA:
sudo apt update
sudo apt install ansible
# create a group in this anmd add private ip address of your node
sudo vi /etc/ansible/hosts
# create a user in all the server 
adduser name
passwd name       (set the password)
visudo           (ansible ALL=(ALL) NOPASSWD: ALL)
su - ansible
 ssh PRIVATE_IP
 ssh-keygen
 ls -a
 cd .ssh
 ls
 ssh-copy-id ansible@172.31.11.169
 ansible demo[0] --list-hosts
 ansible demo[-1] --list-hosts

