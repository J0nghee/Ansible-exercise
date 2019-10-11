Vagrant.configure("2") do |config|
    config.vm.define "node1" do |node1|
        config.vm.box = "centos/7"
    end

    config.vm.define "node2" do |node2|
        config.vm.box = "centos/7"
    end

  ####### Provision #######
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
    ansible.verbose = true
  end
end