SUMMARY -- Ansible, Configuration Management Made Easy: A play in three acts
=================================
Ansible is a configuration management system much like Puppet, Chef or CFEngine which radically simplifies deploying configurations to a multitude of systems.

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

PRESENTER BIOS
===================================
"Goozbach" is Derek Carter; a husband, father, woodworking enthusiast, and active participant in the Open Source Community.
He is the part founder of two Linux users groups, and is a regular presenter at various conferences.
He also actively contributes to several Open Source projects, including some of his own.
Derek has worked as a senior Linux systems administrator for a Fortune 500 company.
He has also worked as a consultant to state agencies, and as a QA engineer for a SAN storage company.
As a Linux instructor, Derek has written course ware, proctored certification exams, and taught classes across the globe for such companies as Red Hat, IBM, Novell, HP, and Lockheed Martin, among others.
Derek currently resides in Athens, Georgia with his family and works as a full-time Linux consultant and instructor.
Find out more at his site[1] or his blog[2].
 
 [1]: http://goozbach.com/
 [2]: http://blog.friocorte.com/
 
 
Thomas Holmquist is a Systems Development Engineer at Georgia Tech. He enjoys planes, trains, automobiles and Linux. Writing Bios are one of his weakpoints.
