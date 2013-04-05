ACT I -- A Sysadmin Has A Problem
=================================
* Manager comes to sysadmin and tells him to setup 4 new DB servers, 5 new webservers, and 2 application servers
* Sysadmin installs each, and does tasks manually
* Manager asks what is taking so long
* Sysadmin explains
* Manager says, "why not use configuration management", here try puppet/cfengine/...
* Sysadmin struggles through mess of config management initial install, gets disheartened and heads to the pub for a break

ACT II -- A Sysadmin Discovers Ansible
======================================
* Sysadmin reads a blog post when he gets back from pub talking about ansible
* Sysadmin installs ansible on testing host, and in 3min is connected to all 11 servers.
* Sysadmin learns about ansible command line as well as playbook.
* Sysadmin writes base playbook and one playbook for each of DB/WEB/APP servers

Act III -- A Happy Manager
==========================
* Manager comes to sysadmin and tells him to add one of each type of server from the spares sitting around.
* Sysadmin comes back in 3min and says "Done!"
* Manager says "HOW?!"
* Sysadmin shows manager the ansible system, a simple base playbook and ad-hoc command line.

***TIME PASSES***

* Manager goes to call sysadmin to ask which version of postgres are installed on all servers, then remembers ansible, and gets command himself.
* Manager adds something to playbook and notifies sysadmin to re-run playbook

EPILOGUE -- What else can ansible do?
===================================
* Cloud stuff -- ec2, openstack
* Show off modules
* ???
