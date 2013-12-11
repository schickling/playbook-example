# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "precise64"
  config.vm.box_url = "http://files.vagrantup.com/precise64.box"

  config.vm.network :private_network, ip: "192.168.33.10"

  config.vm.provision "shell", inline: "echo run playbook"
  
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "ansible.yml"
  end

end
