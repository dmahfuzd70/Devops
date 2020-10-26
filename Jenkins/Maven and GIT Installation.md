Maven Installation
------------------

Step-1

    [ec2-user@ip-172-31-64-105 ~]$ cd /opt
    [ec2-user@ip-172-31-64-105 ~]$ sudo wget https://downloads.apache.org/maven/maven-3/3.6.3/binaries/apache-maven-3.6.3-bin.zip

    [ec2-user@ip-172-31-64-105 ~]$ sudo unzip apache-maven-3.6.3-bin.zip
    [ec2-user@ip-172-31-64-105 ~]$ sudo rm -rf apache-maven-3.6.3-bin.zip

Step-2

[ec2-user@ip-172-31-64-105 ~]$ vi ~/.bashrc

    export M2_HOME=/opt/apache-maven-3.6.3
    
    export M2=$m2_HOME/bin

    export PATH=$m2:$PATH

Reload ~/.bashrc

    source ~/.bashrc

Verify

    mvn --version


GIT Installation
----------------

    [ec2-user@ip-172-31-64-105 ~]$ sudo yum install git -y
    
Verify
    git --version
