vagrant-oracle-tomcat
---------------------

Run `vagrant up` to provision guest vm all-in-one system running Oracle 11g XE and tomcat.

*Tested with the following configuration*

**host system**

* MacOX 10.8
* Virtualbox 4.3.2
* Vagrant 1.3.5

**guest system**

* oracle 5.9 (extra swap space)
* Oracle XE 11g
* Tomcat 7.0.47
* open jdk 1.7

Tomcat
------

The tomcat ansible scripts are based on [ansible-examples/standalone-tomcat](https://github.com/ansible/ansible-examples/tree/master/tomcat-standalone).

Oracle Database
---------------

Unfortunately due to oracle licensing, you will need to accept the license agreement and download the oracle rpm from:

http://www.oracle.com/technetwork/database/database-technologies/express-edition/downloads/index.html

Save the zip file to the download directory.

Basebox
-------
Before you start anything you need a good base box.

I custom built an 'oracle linux 5.9' basebox with extra swap space. You'll need to do the same or find one of the many vagrant baseboxes out there with enough swap space for the oracle SQL installer (complains if there is less than 2048mb of swap).

Instructions
-----------------
If you just want to run this, you can do the following:

1. Install Virtualbox 4.3.2 - https://www.virtualbox.org/wiki/Downloads
2. Install Vagrant 1.3.5 - http://downloads.vagrantup.com/
3. Install Git - http://git-scm.com/downloads
4. Clone this repo
5. Run `vagrant up` from within the project directory


LICENSE
-------
Copyright (c) Kinvey, Inc. 2013


The MIT License (MIT)
