ad_user_management
=========

This role is will create, delete users and update password in Winodws Active Directory

Requirements
------------

Following collection should be availble

collections:
- name: ansible.windows
- name: community.windows

Role Variables
--------------

win_domain_administrator 
win_domain_password
win_domain_server: 

You can create multiple users using ansible list as below. veriable name shoudld be [domain_users_list]
domain_users_list:
  - name: 
    firstname: 
    surname: 
    password: 
    group: 


Tags 
-------------

create_ad_user # create one or more users
delete_ad_user # delete one or more users 
update_ad_user # change password of one or more users

tags:
  - create_ad_user 
  - delete_ad_user
  - update_ad_user

Example Playbook
----------------

ansible-playbook main.yml -t [tag_name] 

License
-------

BSD

Author Information
------------------

KUWAITNET
https://kuwaitnet.com/
