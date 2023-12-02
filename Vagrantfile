Vagrant.configure("2") do |config|
  config.vm.box = "debian/bullseye64"
  config.vm.network "public_network"

  config.vm.define "venus" do |venus|
    venus.vm.hostname = "venus.sistema.sol"
    venus.vm.network "private_network", ip: "192.168.57.102"
    venus.vm.provision "shell", path: "venus.sh"
  end

  config.vm.define "tierra" do |tierra|
    tierra.vm.hostname = "tierra.sistema.sol"
    tierra.vm.network "private_network", ip: "192.168.57.103"
    tierra.vm.provision "shell", path: "tierra.sh"
  end

  config.vm.define "mercurio" do |mercurio|
    mercurio.vm.hostname="mercurio.sistema.sol"
    mercurio.vm.network:public_network ,ip: "192.168.57.101/24"
  end

end

