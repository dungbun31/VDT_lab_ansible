ENV['VAGRANT_SERVER_URL'] = 'https://vagrantcloud.com'
Vagrant.configure("2") do |config|
  box_name = "bento/ubuntu-20.04"

  # app-server-1
  config.vm.define "app_server_1" do |app_server_1|
    app_server_1.vm.provider "vmware_desktop" do |vb_app_server_1|
      vb_app_server_1.memory = 3072
      vb_app_server_1.cpus = 1
    end

    app_server_1.vm.box = box_name
    app_server_1.vm.hostname = "app-server-1"
    app_server_1.vm.network "private_network", ip: "192.168.11.140"
  end
 
  # app-server-2
  config.vm.define "app_server_2" do |app_server_2|
    app_server_2.vm.provider "vmware_desktop" do |vb_app_server_2|
      vb_app_server_2.memory = 1024
      vb_app_server_2.cpus = 1
    end

    app_server_2.vm.box = box_name
    app_server_2.vm.hostname = "app-server-2"
    app_server_2.vm.network "private_network", ip: "192.168.11.141"
  end

  config.vm.define "app_server_1" do |app_server_1|
    app_server_1.vm.provider "vmware_desktop" do |vb_app_server_1|
      vb_app_server_1.memory = 3072
      vb_app_server_1.cpus = 1
    end

    app_server_1.vm.box = box_name
    app_server_1.vm.hostname = "app-server-1"
    app_server_1.vm.network "private_network", ip: "192.168.11.140"
  end
end
