# Ansible-Playbook-With-Variable

--- # Lets Write A File With Variable
- hosts: demo
  vars:
    pkgname: tree
  tasks:
    - name: installation of tree package
      yum:
        name: '{{pkgname}}'
        state: installed
