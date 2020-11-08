##
## Auth R.Othman

Vagrant.configure(2) do |config|
	config.vm.define "devbox" do |devbox|
		devbox.vm.box = "ubuntu/bionic64"
    		#devbox.vm.network "private_network", ip: "192.168.199.9"
    		devbox.vm.hostname = "terraform"
      		devbox.vm.provision "shell", path: "scripts/install.sh"
    		devbox.vm.provider "virtualbox" do |v|
    		  v.memory = 4096
    		  v.cpus = 2
    		end
	end
end
