# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  
  # enable vagrant-env plugin
  # install with `vagrant plugin install vagrant-env` 
  config.env.enable
  
  config.vm.define "etl" do |etl|
    etl.vm.box = "ubuntu/bionic64"
    etl.vm.provision "shell", path: "setup/provision.sh"
    etl.vm.network "private_network", ip: "192.168.33.10"
  end
end