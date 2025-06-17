Vagrant.configure("2") do |config|
  config.vm.box = "centos/stream10"
  config.vm.box_version = "20250520.0"


  # Red
  config.vm.network "public_network", ip: "192.168.56.101"
  config.vm.network "forwarded_port", guest: 80, host: 8080

  # VirtualBox
  config.vm.provider "virtualbox" do |vb|
    vb.memory = "2048"
    vb.cpus = 2
    vb.name = "LEMP-Server"
  end

end
