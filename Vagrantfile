Vagrant.configure("2") do |config| 
    config.vm.box = "bento/ubuntu-22.04" 
    
    config.vm.provider "virtualbox" do |vb| 
        vb.memory = "4024" 
        vb.cpus = "1" 
    end
    config.vm.provision "ansible" do |ansible|
        ansible.become = true
        ansible.verbose = "v"        
        ansible.playbook = "./playbook.yml"
    end
end