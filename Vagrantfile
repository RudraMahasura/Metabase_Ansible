Vagrant.configure("2") do |config|
	config.vm.provider "virtualbox" do |v|
        v.memory = 2048
        v.cpus = 4
    end
	config.vm.box = "ubuntu/focal64"
		config.vm.network 'private_network', ip: '192.168.10.15' 
	  	config.vm.provision 'ansible' do |ans|    ans.playbook = 'Provisioning/metabase_playbook.yml'
 	end
end
