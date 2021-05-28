Install and Configure Ansible

Step-1: Create same user(ansadmin) across all servers and provide password for all users.
Step-2: Provide root privileges to all ansadmin users on all servers.
Step-3: Make sure that PasswordAuthentication yes in all servers under /etc/ssh/sshd_config file.
Step-4: Generate ssh-keys using ssh-keygen command from ansadmin.
Step-5: Copy ssh public key using ssh-copy-id <hostname> from /home/ansadmin/.ssh/ location.
Step-6: Now login to remote server without providing password with the following command:
       ssh user_name@hostname
Step-7: Now we can test connection from Ansible Engine to Manage Node using:
       ansible all -m ping

