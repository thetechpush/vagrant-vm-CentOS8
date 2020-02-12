# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|

	config.vm.define "mytst8srv1" do |mytst8srv1|
    		mytst8srv1.vm.box = "centos/8"
    		mytst8srv1.vm.hostname = "mytst8srv1.example.com"
    		mytst8srv1.vm.network "private_network", ip: "172.42.42.110"
    		mytst8srv1.vm.provider "virtualbox" do |v|
      		  v.name = "mytst8srv1"
      		  v.memory = 2048
      		  v.cpus = 2
      		# Prevent VirtualBox from interfering with host audio stack
      		  v.customize ["modifyvm", :id, "--audio", "none"]
    		end
  	end
end
