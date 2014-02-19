vagrant-shell-lamp
==================

Using shell provision for vagrant box with LAMP

## Usage
1. Clone this repository
2. Inside directory where is Vagrantfile, run `vagrant up`

  log is saved in `./shell/log.txt`

3. Add `192.168.33.10  host.dev` to `/etc/hosts` of host

### This provide:
* Apache2 webserver
  * virtual host http://host.dev
  * mod_rewrite with .htaccess support
  * web directory `/vagrant/www` in guest is shared as ./www in host
* PHP5
* MySQL5 (root password: mysql)
* PHPMyadmin
  * http://host.dev/phpmyadmin

### Remember
* `vagrant ssh` to enter in guest
* `vagrant suspend` to save guest snapshot
* `vagrant halt` to shutdown guest
* `vagrant destroy` to destroy guest if you wish start again