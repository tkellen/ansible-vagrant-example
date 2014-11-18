# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"
NETWORK_IP = "192.168.33.31"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.ssh.forward_agent = true
  config.vm.box = "hashicorp/precise64"
  config.vm.network "private_network", ip: NETWORK_IP
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "ansible.yml"
  end

end
