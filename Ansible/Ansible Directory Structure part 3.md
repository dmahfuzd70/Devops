Ansible Directory Structure
   
    Step-1: To check Ansible File Directory Structure
            [ansadmin@localhost ~]$ tree /etc/ansible
            /etc/ansible
             - ansible.cfg
             - hosts
             - roles
    
    The default location of Inventory file is /etc/ansible/hosts

    Step-2: If we want to our desire inventory file then
    [ansadmin@localhost ~]$ sudo vi myhosts(paste here node server IP)

     In ansible.cfg file change change inventory path

    inventory	= /etc/ansible/myhosts

    Check now 
    [ansadmin@localhost ansible]$ ansible all -m ping

    Step-3: If we dont want to default location of ansible directory

    [ansadmin@localhost ~]$ mkdir my_ansible_working_dir
    [ansadmin@localhost ~]$ cd my_ansible_working_dir
    [ansadmin@localhost my_ansible_working_dir]$ cp -rpP /etc/ansible/* .
    [ansadmin@localhost my_ansible_working_dir]$ ls -lrt
    [ansadmin@localhost my_ansible_working_dir]$ rm hosts
    [ansadmin@localhost my_ansible_working_dir]$ ls
    [ansadmin@localhost my_ansible_working_dir]$ sudo vi inventory(paste here node server IP)
    [ansadmin@localhost my_ansible_working_dir]$ vi ansible.cfg
        inventory	= ./inventory
    [ansadmin@localhost my_ansible_working_dir]$ ansible all -m ping

    Step-4: If we dont mention inventory file in ansible.cfg then
    [ansadmin@localhost my_ansible_working_dir]$ ansible all -m ping -i inventory
