# rpiclusteroperationautomation

Very simple Ansible playbooks to manage the Raspberry PI clsuter nodes (Reboot, Shutdown, Update and Upgrade) remotly from the master node.


# Prerequisite
- [Ansible](https://www.ansible.com)
- sshpass

# Steps to run the Playbook

## Clone the repository

Clone this repository to your master or monitoring node

`git clone https://github.com/deepaksks/rpiclusteroperationautomation.git`

## Edit the host file

Update the password for the PI's and IP addresses of the Pi's running in the cluster
 

## To run a playbook

### Shutdown

Executing the below playbook will Shutdown all the Raspberry PI's in the cluster

`ansible-playbook playbooks/shutdownnodes.yml -i hosts`


### Reboot

Executing the below playbook will Reboot all the Raspberry PI's in the cluster

`ansible-playbook playbooks/rebootnodes.yml -i hosts`
