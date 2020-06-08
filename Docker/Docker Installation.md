Prerequisite for Docker installation:-

1> OS must be 64bit (Use command uname -m to check bit)
2> Kernel must be more then 3.10 (Use uname -r to check the kernel version)
Documentation for docker :-
https://docs.docker.com/
First check if any docker is preinstalled in the server by using the command “docker –
version” or docker -v , if any docker exists then first remove all docker related instance
using below command:-
yum remove -y docker docker.io docker-engine docker-ce docker-ee
