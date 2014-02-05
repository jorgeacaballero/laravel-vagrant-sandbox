laravel-vagrant-sandbox
=======================

A simple Laravel setup in Vagrant, project included!


Usage
-----

**Requirements**

- Vagrant 1.2.7 or higher
- VirtualBox 4.2.16 or higher

**Installation**

```bash
git clone https://github.com/jorgeacaballero/laravel-vagrant-sandbox.git
cd laravel-vagrant-sandbox
vagrant up 
```
Wait for the download to finish. Once the VM is running, connect to the machine via ssh and install dependencies:

```bash
cd laravel-vagrant-sandbox
vagrant ssh

...

vagrant@precise32:~$ cd /vagrant/pymeERP/
vagrant@precise32:/vagrant/pymeERP$ composer install

```

Once done go to `http://localhost:4567` and you should recive the "You have arrived." message from Laravel.

**Troubleshoot**

If you run into a white page when loading `http://localhost:4567`, on your host computer change the access permissions to the pymeERP folder:

```bash
cd laravel-vagrant-sandbox
sudo chmod -R 777 pymeERP
```

**Usefull hints**

You can change the project name by manually renaming it's folder and changing the DocumentRoot in the default site config:

```bash
sudo vi /etc/apache2/sites-available/default
```

MySQL root password: `root` :O


**Box Info**

- Ubuntu 12.04 LTS (GNU/Linux 3.2.0-23-generic-pae i686)
- MySql 5.5.35-0ubuntu0.12.04.2
- Laravel 4.1
- Composer bac8b81d416133bdc5d468c71e49685bab786af4
- Apache 2.2.22
- PHP 5.3.10-1ubuntu3.9 with Suhosin-Patch
- Zend Engine v2.3.0


Credits
-------

Thanks Seich for your help tackling down the permissions problem. [Seich's Github](https://github.com/Seich)

Other references:

- [Jeffrey Way's Script](https://github.com/JeffreyWay/Vagrant-Setup)
- [Setting Up Vagrant With Laravel 4](http://culttt.com/2013/06/17/setting-up-vagrant-with-laravel-4/)


