Ansible LEMP Stack Server Setup
======================================================
This play book will install lemp stack(Linux, Nginx, MySQL, PHP) with Composer, Redis and Supervisor on target host.
Playbook tested only target machine operating system `Ubuntu Focal Fossa (20.04) LTS`.

Requirement
-----------
* Install ansible on controller machine - [ansible installation](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) 
* Add controller machine's public key ``~/.ssh/id_rsa.pub`` in target host authorized_keys ``~/.ssh/authorized_keys``

Installation
------------

Clone the repository on master controller machine

    git clone https://github.com/ashokdevatwal/ansible-lemp-stack.git
    
Change current working directory to ansible-lemp-stack

    cd ansible-lemp-stack
    
Run Playbook

    ansible-playbook lemp-stack.yaml --extra-vars "target_host=host_name"


## Versions that will install

| Software   | Version |
| ---------- | ------- |
| nginx      | latest  |
| MySQL      | latest  |
| PHP        | 7.4     |
| redis      | latest  |
| Composer   | latest  |
| Supervisor | latest  |



Author
------

* Ashok Devatwal <ashokdev78@gmail.com>
* Twitter: *[@ashokdev_ars](https://twitter.com/ashokdev_ars)*

