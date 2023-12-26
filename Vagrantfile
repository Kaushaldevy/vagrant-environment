# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  # Specify the base box to use
  config.vm.box = "almalinux/9"

  # Define the configuration for the "web1" VM
  config.vm.define "web1" do |web1|
    # Provider-specific settings for VirtualBox
    web1.vm.provider "virtualbox" do |vb|
      vb.cpus = 2
      vb.memory = 1024
    end

    # Private network settings
    web1.vm.network :private_network, ip: "192.168.2.115"

    # Hostname for the VM
    web1.vm.hostname = "webserver-1"
  end
end