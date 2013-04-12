SUMMARY -- Ansible, Configuration Management Made Easy: A play in three acts
=================================
Ansible is a configuration management system similar to Puppet, Chef or CFEngine which radically simplifies deploying configurations to a multitude of systems.

Come learn how to install, configure, and use one of the simplest and easy to use (but still very powerful) Configuration Management tools. 
This presentation is a real-world example done in a fun and entertaining format -- The Three-Act Play.

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

Forking
=======
This presentation can be fully re-done by anyone and there are some tools present to help with that.

## The Servers
The directory `presentation-setup-playbooks/` contains a fully tested ansible playbook for setting up the same environment used for the course.  Yes, we are bootstrapping an Ansible talk using Ansible.  It requires 7 servers (We used virtualbox guests with two nics, one using nat, the other using a host-only network).  By default the above playbook sets up the following:
* ansible.example.com -- the ansible server to manage the rest -- 10.200.45.100
 * The file `kickstarts/ansible-server-kickstart.cfg` was used to create the server 'ansible.example.com' and the remainder of the servers were created as 'linked clones' of the ansible server, ***AFTER*** the ansible server was updated using `yum update`.
* web servers
 * web1.example.com -- 10.200.45.10
 * web2.example.com -- 10.200.45.11
 * db1.example.com -- 10.200.45.20
 * db2.example.com-- 10.200.45.21
 * app1.example.com -- 10.200.45.30
 * app2.example.com -- 10.200.45.31

