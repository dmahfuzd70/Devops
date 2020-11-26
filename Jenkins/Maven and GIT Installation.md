Maven Installation
------------------

Step-1

    [ec2-user@ip-172-31-64-105 ~]$ cd /opt
    [ec2-user@ip-172-31-64-105 ~]$ sudo wget https://downloads.apache.org/maven/maven-3/3.6.3/binaries/apache-maven-3.6.3-bin.zip

    [ec2-user@ip-172-31-64-105 ~]$ sudo unzip apache-maven-3.6.3-bin.zip
    [ec2-user@ip-172-31-64-105 ~]$ sudo rm -rf apache-maven-3.6.3-bin.zip

Step-2

[ec2-user@ip-172-31-64-105 ~]$ vi ~/.bashrc
    
    export PATH=/opt/maven3/bin:$PATH

    
    export M2_HOME=/opt/maven3
    
    export M2=$M2_HOME/bin

    export PATH=$M2:$PATH

Reload ~/.bashrc

    source ~/.bashrc

Verify

    mvn --version


GIT Installation
----------------

    [ec2-user@ip-172-31-64-105 ~]$ sudo yum install git -y
    
Verify
    git --version
