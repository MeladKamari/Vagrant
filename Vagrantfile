Vagrant.configure("2") do |config|
  config.vm.provider "virtualbox" do |v|
    v.memory = 4096
    v.cpus = 2
    v.gui = true
  end
  config.vm.hostname = "master23"
  config.vm.box = "generic/ubuntu2010"
  #config.vm.synced_folder=""
  config.vm.network "private_network", ip: "192.168.125.125"
  config.vm.provision "shell", path: "bootstrap.sh"
end