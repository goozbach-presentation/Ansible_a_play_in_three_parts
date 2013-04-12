ACT I -- A Sysadmin Has A Problem
=================================
* Manager comes to sysadmin and tells him to setup 1 new DB server, 1 new webservers, and 1 application servers
* Sysadmin installs each, and does tasks manually
* Manager asks what is taking so long
* FIRST DEMO, configure apache -- by hand
* Sysadmin explains
* Manager says, "why not use configuration management", here try puppet/cfengine/...
* Sysadmin struggles through mess of config management initial install, gets disheartened and heads to the pub for a break
* puppet docs -- RAL http://docs.puppetlabs.com/learning/ral.html

ACT II -- A Sysadmin Discovers Ansible
======================================
* Sysadmin reads a blog post when he gets back from pub talking about ansible
* **START DEMOS HERE**
** http://ansible.cc/docs/gettingstarted.html#your-first-commands
* Sysadmin installs ansible on testing host, and in 3min is connected to all 3 servers.
* Sysadmin learns about ansible command line
** ad-hoc raw install simple-json
** Setup module
** Add ssh-key for root access
* Sysadmin learns about the ansible playbooks
* Sysadmin writes base playbook
* Sysadmin writes one playbook for each of DB/WEB/APP servers
** Base playbook
*** ntp installed and configured
*** ntpdate run
*** for each 
**** Users added (goozbach fignew)
**** ssh key for goozbach fignew

** DB Playbook
*** include baseimage tasks --tags common
*** install mysql
*** enable mysql
*** start mysql
*** handler restart mysql
*** mysql create user
*** mysql create db

** Web Playbook
*** include baseimage --tags common
*** install httpd
*** configure hostname in httpd.conf (template) 
*** httpd started
*** httpd enabled
*** restart/reload httpd handler
*** git repo of web content

** APP playbook
*** include baseimage --tags common
*** include web --tags apache
*** install php
*** get_url for app content

Act III -- A Happy Manager
==========================
* Manager comes to sysadmin and tells him to add one of each type of server from the spares sitting around.
* 
* Sysadmin comes back in 3min and says "Done!"
* Manager says "HOW?!"
** Show site playbook.

***TIME PASSES***

* Manager goes to call sysadmin to ask which version of mysql are installed on all servers, then remembers ansible, and gets command himself.
* Manager adds something to playbook and notifies sysadmin to re-run playbook

EPILOGUE -- What else can ansible do?
===================================
* Show off modules
** Cloud stuff -- ec2, openstack
* with_items
* only_if
* delegate_to 
* register
* config file
* cowsay Thomas "this is great, but something's missing...." -- Derek "I Know COWS!"
* derek installs cowsay, re-runs playbook
* Thomas -- "THAT'S IT! PERFECT!"

