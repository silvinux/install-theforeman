install-theforeman
=========
A role to install theforeman ansible modules on a disconnected enviroment.

Requirements
------------
Ansible 2.9 installed. The folowging packages version will be used:
 - python2-apypie-0.2.1-1.el7.noarch.rpm  
 - theforeman-foreman-0.7.0.tar.gz


Role Variables
--------------
theforemanpath: /root/test

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

---
- hosts: theforeman
  gather_facts: yes
  become: yes
  become_method: sudo
  become_user: root
  remote_user: ansible
  vars: 
    theforemanpath: /root/test
  roles:
    - role: ../roles/install-theforeman

License
-------

GPLv3

Author Information
------------------

silvinux - silvinux7@gmail.com
