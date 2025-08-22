Vagrant.configure("2") do |config|
  config.vm.define "kali-machine1" do |subconfig|
    subconfig.vm.box = "kalilinux/rolling"
    subconfig.vm.hostname = "kaliVM-1"

    # VMware provider settings
    subconfig.vm.provider "vmware_desktop" do |v|
      v.memory = 2048
      v.cpus = 1
    end

    # Ansible provisioning
    subconfig.vm.provision "ansible_local" do |a|
      a.playbook = "setupkali.yml"
    end
  end
end
