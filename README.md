# devops-study-project-vm
Private project to study DevOps tools and methodology

Automatically provision a KVM virtual machine (managed through libvirt) on an Ubuntu Desktop 20.04 LTS/22.04 LTS. Also included is a playbook that allows tearing down created environment.

---
For these playbooks to work on your ansible control node you'll need: 
  ansible-core
  ansible-galaxy collections:
    - community.general
    - community.libvirt
  ansible-galaxy roles:
    - geerlingguy.swap (https://galaxy.ansible.com/geerlingguy/swap) - install with 'ansible-galaxy install geerlingguy.swap')
  packages:
    - cloud-image-utils
  (to be continued)
---
