# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "bento/centos-7.4"
  config.vm.hostname = 'cent'
  config.ssh.forward_x11 = true

  # config.vm.network "forwarded_port", guest: 80, host: 8080

  # config.vm.synced_folder "../data", "/vagrant_data"

  config.vm.provider "virtualbox" do |vb|
    #vb.gui = true
    vb.memory = "1024"
    vb.cpus = "2"
  end

  config.vm.provision "shell", path: 'install-pkgs.sh'
  #config.vm.provision "shell", path: 'install-xfce.sh'
end
