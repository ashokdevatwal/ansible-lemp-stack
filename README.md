Ansible LEMP Stack Server Setup
======================================================
This play book will install lemp stack on target host . make sure your controller machine have ansible installed.

 
Installation
------------

Clone the repository on master controller machine

    git clone https://github.com/ashokdevatwal/ansible-lemp-stack.git

    cd ansible-lemp-stack

    ansible-playbook lemp-stack.yaml --extra-vars "target_host=host_name"


This playbook will install following services 
 - PHP
 - Composer
 - MySql
 - Redis
 - Nginx
 - Supervisor



Author
------

* Ashok Devatwal <ashokdev78@gmail.com>
* Twitter: *[@ashokdev_ars](https://twitter.com/ashokdev_ars)*

