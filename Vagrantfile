Vagrant.configure("2") do |config|

  config.vm.define "weber01" do |weber01|
    weber01.vm.box = "ubuntu/xenial64"
	weber01.vm.hostname = "Ansibleclientwebserver"
	weber01.vm.network "private_network", ip: "192.168.33.11"
	
  end

  config.vm.define "dbsrv01" do |dbsrv01|
    dbsrv01.vm.box = "geerlingguy/centos7"
	dbsrv01.vm.network "private_network", ip: "192.168.33.10"
	dbsrv01.vm.hostname = "Ansibleclientdbserver"
	dbsrv01.vm.provider "virtualbox" do |vb|
        vb.memory = "512"
	   
    end
  end
end

