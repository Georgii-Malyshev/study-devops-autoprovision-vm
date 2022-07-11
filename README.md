# ansible-autoprovision-vm
Small Ansible-based project that can automatically provision a KVM virtual machine (managed through libvirt) on an Ubuntu Desktop 20.04 LTS/22.04 LTS. Also included is a playbook that allows tearing down created environment.

Variables that define various parameters of the VM to be provisioned are defined in an YAML-format inventory file. They should be set before running any of the playbooks.

For these playbooks to work on an Ansible control node the following dependencies must be met: 
- ansible-core
- ansible-galaxy collections:
  - community.general
  - community.libvirt
- ansible-galaxy roles:
  - geerlingguy.swap (https://galaxy.ansible.com/geerlingguy/swap) - install with 'ansible-galaxy install geerlingguy.swap')
- packages:
  - cloud-image-utils

With Ansible installed, you can install Ansible Galaxy collection and roles required by this project by running: \
\
ansible-galaxy install -r requirements.yml