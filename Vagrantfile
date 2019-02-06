# encoding: UTF-8
Vagrant.configure("2") do |config|

#speficy the base box
config.vm.box = "centos/7"
config.vm.network :public_network, ip: "192.168.0.50"
	config.vm.provision"shell" do |s|
	s.path="provision/set_hostname.sh"
	end
config.ssh.insert_key = 'true'
config.vm.provider "virtualbox" do |v|
v.name = "rancher.test"
	end
end