Install and Configure Ansible

       Step-1: Create same user(ansadmin) across all servers and provide password for all users.
              [root@desktopX ~]# useradd ansadmin
              [root@desktopX ~]# passwd ansadmin
              
       Step-2: Provide root privileges to all ansadmin users on all servers.
              [root@desktopX ~]# visudo 

               :set nu

               92   root    ALL=(ALL)    ALL
               93   ansadmin  ALL=(ALL)    ALL    ; mahedi allow for any command

              :x (save and exit)
       
       Step-3: Make sure that PasswordAuthentication yes in all servers under /etc/ssh/sshd_config file.
               Restart service sshd following command:
               sudo service sshd restart
               
       Step-4: Generate ssh-keys using ssh-keygen command from ansadmin.
               [root@hostX .ssh]# ssh-keygen  ; (Enter 3 Times)
       
       Step-5: Copy ssh public key using ssh-copy-id <hostname> from /home/ansadmin/.ssh/ location.
               [root@hostX .ssh]# ssh-copy-id user1@172.25.11.200+X
               
       Step-6: Now login to remote server without providing password with the following command:
              ssh user_name@hostname
              
       Step-7: Now we can test connection from Ansible Engine to Manage Node using:
              ansible all -m ping

