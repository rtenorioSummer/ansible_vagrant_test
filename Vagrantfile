Vagrant.configure(2) do |config|
  config.vm.box = "centos/7"
  config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.network "private_network", ip: "123.123.31.2"
	config.vm.provision :ansible do |ansible|
		ansible.playbook= "playbooks/testnode/playbook.yml"
	end
	
end
