Install MSSQL Standalone with SSMS
=========

This role will Check the necessary file path and exe is available and install prerequisites  

Requirements
------------
MSSQL and SSMS need to be downloaded because this playbook is to conduct offline installation altho this can develop as an online installation environment easily  

The following collection should be available
collections:
- name: ansible.windows
- name: community.windows

Role Variables
--------------
- installation_path: 'C:\SQL_2016'
- sql_instance_name: "{{ ansible_hostname }}"
- download_path: 'C:\Users\Administrator\Downloads\SQLServer2016SP2-FullSlipstream-x64-ENU\'
- playbook_dir: '/etc/ansible/roles/mssql_install'

Tags 
-------------
There are no tags designed 


Example Playbook
----------------

ansible-playbook main.yml 

License
-------

BSD

Author Information
------------------

KUWAITNET
https://kuwaitnet.com/
