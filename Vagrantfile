Vagrant.configure("2") do |config|
	config.vm.box = "ubuntu/xenial64"
	
	# Docker Provisioner
	config.vm.provision "docker" do |d|
		d.pull_images "ubuntu:14.04"
	end			
	
end
