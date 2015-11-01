# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.define "centos", primary: true do |centos|
    centos.vm.box = "puppetlabs/centos-7.0-64-nocm"
    centos.vm.network "private_network", ip: "192.168.33.10"
  end
  config.vm.define "ubuntu", autostart: false do |ubuntu|
    ubuntu.vm.box = "puppetlabs/ubuntu-14.04-64-nocm"
    ubuntu.vm.network "private_network", ip: "192.168.33.11"
  end
end
