Vagrant.configure("2") do |config|

    config.vm.box = "ubuntu/trusty64"

    config.vm.network :private_network, ip: "192.168.33.101"

    config.vm.provision "ansible" do |ansible|
        ansible.playbook = "playbook.yml"
    end

    config.vm.synced_folder "./", "/vagrant/web"

end
