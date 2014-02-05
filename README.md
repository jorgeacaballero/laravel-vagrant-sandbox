laravel-vagrant-sandbox
=======================

A simple Laravel setup in Vagrant, project included!


Usage
-----

**Requirements**

- Vagrant 1.2.7 or higher

**Installation**

```bash
git clone https://github.com/jorgeacaballero/laravel-vagrant-sandbox.git
cd laravel-vagrant-sandbox
vagrant up 
```

Once done go to `http://localhost:4567` and you should recive the "You have arrived." message from Laravel.

**Troubleshoot**

If you run into a white page when loading `http://localhost:4567`, on your host computer change the access permissions to the pymeERP folder:

```bash
cd laravel-vagrant-sandbox
sudo chmod -R 777 pymeERP
```

Credits
-------

Thanks Seich for your help tackling down the permissions problem. [Seich's Github](https://github.com/Seich)

Other references:

- [https://github.com/JeffreyWay/Vagrant-Setup](https://github.com/JeffreyWay/Vagrant-Setup)
- [https://gist.github.com/fideloper/7074502](https://gist.github.com/fideloper/7074502)
- [Setting Up Vagrant With Laravel 4](http://culttt.com/2013/06/17/setting-up-vagrant-with-laravel-4/)
- [How to Install the Latest Version of PHP 5.5 on Ubuntu](http://www.dev-metal.com/how-to-setup-latest-version-of-php-5-5-on-ubuntu-12-04-lts/)


