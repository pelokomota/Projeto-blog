Vagrant.configure("2") do |config|
  config.vm.box = "generic/ubuntu2004"
  config.vm.provider "virtualbox" do |v|
    v.memory = 1024
  #config.ssh.insert_key = false
    end  

  config.vm.define "wordpress" do |m|
    m.vm.network "private_network", ip: "172.17.177.40"
    end

  config.vm.define "mysql" do |mysql|
    mysql.vm.network "private_network", ip: "172.17.177.41"
    end
end