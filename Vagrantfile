Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial32"

  config.vm.provider "virtualbox" do |v|
    v.memory = 256
    v.cpus = 1
  end

  config.vm.provision "file", source: "./snx_install_linux30.sh", destination: "~/snx_install_linux30.sh"
  config.vm.provision "shell", path: "install.sh"

end
