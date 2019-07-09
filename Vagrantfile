# -*- mode: ruby -*-
# vi: set ft=ruby :
# This Vagrantfile aim to be used as a Kuzzle plugin development plateform.
# Put it in your Kuzzle plugin directory root
Vagrant.configure("2") do |config|
  config.vm.box = "kuzzle/plugin-dev"
  config.vm.box_version = "1.8.4"

  # Kuzzle API port
  config.vm.network "forwarded_port", guest: 7512 , host: 7512

  config.vm.synced_folder "./", "/home/vagrant/plugin"
  config.vm.provider "virtualbox" do |vb|
  # Customize the amount of memory on the VM:
    vb.memory = "2048"
	vb.customize [ "modifyvm", :id, "--uartmode1", "disconnected" ]
  end
end