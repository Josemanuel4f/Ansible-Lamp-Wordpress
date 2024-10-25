VAGRANTFILE_API_VERSION= "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
    config.vm.define "loadbalancer" do |app|
        app.vm.box = "bento/ubuntu-16.04" 
        app.vm.hostname = "loadbalancer" 
        app.vm.synced_folder ".", "/vagrant", disabled: true
        app.vm.network :private_network, ip: "192.168.56.11"
        app.vm.provider "VirtualBox" do |v|
            v.memory = 512
            v.cpus = 1
        end
    end
    config.vm.define "webserver-one" do |app|
        app.vm.box = "bento/ubuntu-16.04" 
        app.vm.hostname = "webserver-one" 
        app.vm.synced_folder ".", "/vagrant", disabled: true
        app.vm.network :private_network, ip: "192.168.56.12"
        app.vm.provider "VirtualBox" do |v|
            v.memory = 512
            v.cpus = 1
        end
    end
    config.vm.define "webserver-two" do |app|
        app.vm.box = "bento/ubuntu-16.04" 
        app.vm.hostname = "webserver-two" 
        app.vm.synced_folder ".", "/vagrant", disabled: true
        app.vm.network :private_network, ip: "192.168.56.13"
        app.vm.provider "VirtualBox" do |v|
            v.memory = 512
            v.cpus = 1
        end
    end
    config.vm.define "dbserver" do |app|
        app.vm.box = "bento/ubuntu-16.04" 
        app.vm.hostname = "dbserver" 
        app.vm.synced_folder ".", "/vagrant", disabled: true
        app.vm.network :private_network, ip: "192.168.56.14"
        app.vm.provider "VirtualBox" do |v|
            v.memory = 512
            v.cpus = 1
        end
    end
    config.vm.define "controller" do |app|
        app.vm.box = "bento/ubuntu-16.04" 
        app.vm.hostname = "controller" 
        app.vm.synced_folder ".", "/vagrant", disabled: true
        app.vm.network :private_network, ip: "192.168.56.15"
        app.vm.provider "VirtualBox" do |v|
            v.memory = 512
            v.cpus = 1
        end
    end
end