Vagrant.configure("2") do |config|


 config.vm.define "ubuntu81" do |ubuntu81|
    ubuntu81.vm.box = "bento/ubuntu-20.04"
    ubuntu81.vm.network "private_network", ip: "192.168.43.81"
     ubuntu81.vm.provider "virtualbox" do |vb|

     vb.memory = "2048"
     vb.cpus = "1"
     end

     ubuntu81.vm.provision "ansible" do |ansible|
       ansible.verbose="v"
       ansible.playbook="initial_provision.yaml"
       ansible.extra_vars="credentials.yaml"
     end
end

end
