Vagrant.configure("2") do |config|
    config.vm.define "node1" do |node1|
        node1.vm.box = "centos/7"
        node1.vm.network "public_network"
        #node1.vm.network :"forwarded_port", guest: 2376, host: 3000
        node1.vm.hostname = "node1"
    end

    config.vm.define "node2" do |node2|
        node2.vm.box = "centos/7"
        node2.vm.network "public_network"
        #node2.vm.network :"forwarded_port", guest: 2376, host: 3001
        node2.vm.hostname = "node2"
    end

  ####### Provision #######
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
    ansible.verbose = true
  end
end