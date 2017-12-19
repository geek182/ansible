Role Name
=========

Install PHP-FPM and some base packages like :
- php (really ?)
- mbstring
- xml
- pdo

Requirements
------------

in this version of role i used RedHat(Centos) or Amazon Linux like a requiremente, why ???? some packages in amz has a different name.

Role Variables
--------------

Need pass a php version, for example:
ansible-playbook custom-role.yml -e roles=php-fpm -e "version=71"

Dependencies
------------

Not yet

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: php-fpm, version: 71 }
         
Or using a custom-role: 
ansible-playbook custom-role.yml -e roles=php-fpm -e "version=71"


License
-------

BSD

Author Information
------------------
Leandro Azevedo
@geek182
