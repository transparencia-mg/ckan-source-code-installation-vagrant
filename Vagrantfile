# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  
  # enable vagrant-env plugin
  # install with `vagrant plugin install vagrant-env` 
  config.env.enable
  
  config.vm.define "ckan" do |ckan|
    ckan.vm.box = "ubuntu/bionic64"
    ckan.vm.provision "shell", path: "setup/provision.sh"
    ckan.vm.network "private_network", ip: "192.168.33.10"
  end
end