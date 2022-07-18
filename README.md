Install NGINX
=========

This is playbook is responsible by install of the application NGINX to O.S CentOS and Ubuntu in all versions:


Requirements
------------

This is playbook has necessity of access remote ssh to hosts destination and add the IPs or hostname of the hosts at file *inventory-hosts* witch there is at  project, the IPs separete for *enter*.

Ex inventory-hosts:
```
[hosts-nginx]
10.0.0.123
serverweb
```

NGINX Variables
--------------

The project has variables definitions at files in directory *vars*.

    - vars
      - main.yml

Example of runnig Playbook
----------------

```
$ ansible-playbook -i inventory-hosts play.yml
```
*Please adding files at directory "files" to delivery at server-host*