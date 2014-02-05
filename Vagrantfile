# -*- mode: ruby -*-
# vi: set ft=ruby :

## CREATED BY SERGIO DIAZ & JORGE CABALLERO

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
    config.vm.box = "laravel"
    config.vm.box_url = "https://googledrive.com/host/0B_VtmPiBRE1xTUt5aTFaWnhmVjg/laravel.box"
    config.vm.network :forwarded_port, host: 4567, guest: 80
    config.vm.synced_folder ".", "/vagrant", :mount_options => ["dmode=777", "fmode=777"]
end
