## Configuration Management Tool
  1. Puash based
              
    The nodes are dynamically updated with the configurations that are present in the server.
    1. Ansible 
    
  2. Pull Based
        
    Centralized server pushes the configurations on the nodes.
    1. Chef
    2. Puppet


## Chef
    -> Chef is a Company and the name of a configuration management tool written in Ruby and Erlang
    -> Founded by Adam Jacobs in year 2009
    -> Actual Name was 'Marionette' later renamed to 'Chef'
    -> On April 2, 2019, the Company announced that all their products are now open source under
    the Apache 2.0 License
    -> Chef is used by Facebook, AWS opsworks, HP Public Cloud etc
    -> Chef is an administration tool whatever System admins used to do manually, now we are 
      automating all those task by using Chef

## Advantage of Control Management Tool
    -> Complete Automation
    -> Increase uptime
    -> Improve Performance
    -> Ensure Compliance
    -> Prevent Errors 
    -> Reduce Cost


## Chef Architectuore and process

<img src="/Chef/Images/1.png" alt="Chef Directory" width="700" height="350">

<img src="/Chef/Images/2.png" alt="Chef Directory" width="700" height="350">

### Components of Chef

Workstation
    
    ->Workstation are personal Computer or Virtual server 
      wherer all Configuration Code is Created, tested or Changed.
    ->Devops engineer actually sits here and write codes. This code is
      called Receipe. A collection Receipe known as Cookbook
    -> Workstation communicate with the Chef server using knife
    -> Knife is a command line tool that uploads the Cookbook to the
       server.

Chef-Server

    ->The Chef-Server is a middle-man between workstation and the nodes
    ->All Cookbooks are stored here
    ->Server may be hosted locally or remote

Node

    ->Nodes are the systems that require the Configuration
    ->Ohai Fetches the current state of the node located
    ->Node communicate with the Chef-Server using the Chef-Client
    ->Each node can have a different Configuration required
    ->Chef-Client is installed on every node.


Summary

<img src="/Chef/Images/3.png" alt="Chef Directory" width="600" height="300">

<img src="/Chef/Images/4.png" alt="Chef Directory" width="600" height="300">
