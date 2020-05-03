# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.define "metropolitana" do |metropolitana|
    metropolitana.vm.box = "generic/ubuntu1804"
    metropolitana.vm.box_check_update = false
    metropolitana.vm.network "private_network", ip: "192.168.0.2"
    metropolitana.vm.hostname = "metropolitana"
    config.vm.synced_folder ".","/home/vagrant/Documentos"
     config.vm.provider "virtualbox" do |v|
        v.memory = 1024
        v.cpus = 2
  end
end

  config.vm.define "ansiblemetropolitana" do |ansiblemetropolitana|
    ansiblemetropolitana.vm.box = "generic/ubuntu1804"
    ansiblemetropolitana.vm.network "private_network", ip: "192.168.0.254"
    ansiblemetropolitana.vm.hostname = "ansiblemetropolitana"
    config.vm.synced_folder ".","/home/vagrant/Documentos"
    config.vm.provider "virtualbox" do |v|
        v.memory = 1024
        v.cpus = 2
  end
end
end
