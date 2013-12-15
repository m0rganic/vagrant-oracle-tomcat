vagrant-oracle
-----------------

Vagrant box with oracle xe setup using ansible.

Oracle Databse
--------------

Unfortunately due to oracle licensing, you will need to accept the license agreement and download the oracle rpm from:

http://www.oracle.com/technetwork/database/database-technologies/express-edition/downloads/index.html

Save the zip file to the download directory.

Basebox
-------

I custom built my own 'oracle linux 5.9' basebox with extra swap space. You'll need to do the same or find one of the many vagrant baseboxes out there (centOS, oraclelinux, rhel) and make sure to add swap space because the oracle installer will complain if swap is less than 2048mb.

Instructions
-----------------
If you just want to run this, you can do the following:

1. Install Virtualbox 4.3.2 - https://www.virtualbox.org/wiki/Downloads
2. Install Vagrant 1.3.5 - http://downloads.vagrantup.com/
3. Install Git - http://git-scm.com/downloads
4. Clone this repo
5. Run `vagrant up` from within the project directory
