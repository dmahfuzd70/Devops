Ansible Configuration
---------------------

Step-1: Configure Password Less Authentication
    
    [root@master ~]# ssh-keygen
    [root@master ~]# ssh-copy-id root@192.168.198.132
    [root@master ~]# ssh-copy-id ansadmin@192.168.198.132
    [root@master ~]# su ansadmin
    [ansadmin@master ~]$ ssh-keygen
    [ansadmin@master ~]$ ssh-copy-id root@192.168.198.132
    [ansadmin@master ~]$ ssh-copy-id ansadmin@192.168.198.132
