Vagrant.configure(2) do |config|
  config.vm.box = "centos/7"
  config.vm.hostname="testansi"
  config.vm.define "testansi"
  config.vm.network "private_network", ip: "123.123.31.2"
	config.vm.provision :ansible do |ansible|
		ansible.playbook= "playbooks/testnode/playbook.yml"
    ansible.extra_vars = {
      vm_specific: "xxx"
    }
	end

end
