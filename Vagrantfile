Vagrant.configure("2") do |config|
    config.vm.box = "centos/7"

  ####### Provision #######
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
    ansible.verbose = true
  end
end