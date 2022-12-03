Role Name: user_groups
======================

This is Ansible role for managing local user groups. It doesn't manage a LDAP user groups. 

The role supports next use cases:

1. Host based management of local user groups.

2. Hosts group based management of local user groups (if one is not true).

3. Ansible OS Family based management of local user groups (if one and two is not true). 

Requirements
------------
None.

Role Variables
--------------

1. ```min_gid``` (integer var) defines min GID for local user group.

2. ```known_common_groups, known_host_groups, known_hostgroup_groups``` (list vars) 
   define groups that are not removed by this role. These groups are known and are ignored.
   The common is based on OS fmaily. 

3. ```managed_common_groups, managed_host_groups, managed_hostgroup_groups``` (list vars) 
   define groups that need to be present on a host. The common is based on OS fmaily. 

You can add more families is the var folder.  

Dependencies
------------
None

Example Playbook
----------------
See test folder. 

Author Information
------------------
Zarko D.

License
--------
Hello! I’ve created this, and placed it in the Public domain. 
There is no ownership such as copyright, trademark, patent, and there is no warranty. 
Thank you.
