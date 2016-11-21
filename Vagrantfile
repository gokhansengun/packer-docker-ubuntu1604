# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.ssh.insert_key = false

  config.vm.define "virtualbox" do |virtualbox|
    virtualbox.vm.hostname = "virtualbox-docker-ubuntu1604"
    virtualbox.vm.box = "file://builds/virtualbox-docker-ubuntu1604.box"
    ## virtualbox.vm.network :private_network, ip: "172.16.3.2"

    config.vm.provider :virtualbox do |v|
      v.gui = false
      v.memory = 1024
      v.cpus = 1
    end
    
    config.vm.provision "shell", inline: "echo Hello, World"
  end
end
