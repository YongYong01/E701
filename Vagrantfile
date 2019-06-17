Vagrant.configure("2") do |config|
	config.vm.box = "ubuntu/xenial64"
	config.vm.network "forwarded_port", guest:80, host:8080, auto_correct: true
  	config.vm.network "forwarded_port", guest:8081, host:8081, auto_correct: true
  	config.vm.network "forwarded_port", guest:8082, host:8082, auto_correct: true
  	config.vm.network "forwarded_port", guest:3306, host:3306, auto_correct: true  
for i in 32760..32780
    	config.vm.network :forwarded_port, guest: i, host: i
end	
	# Docker Provisioner
	config.vm.provision "docker" do |d|
		d.pull_images "ubuntu:14.04"
	end			
	
end
