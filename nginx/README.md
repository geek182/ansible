Role Name
=========

Install nginx in Redhat based OS

Requirements
------------

Before use this role you should upload a config do your app see "Templates Files"  to more details

Role Variables
--------------

nginx_app_config: Specific config to your app  
nginx_main_file: Main config file to nginx, if not pass will use default "config-default-nginx.j2"  

Dependencies
------------

Nothing 

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: nginx, nginx_app_config: config-default-nginx.j2, app_name: app-name }

#using custom-role.yml
ansible-playbook custom-role.yml -e roles=nginx -e "nginx_app_config=config-default-nginx.j2" -e "app_name=portal_conteudo"

License
-------

BSD

Author Information
------------------

Leandro Azevedo  
@geek182