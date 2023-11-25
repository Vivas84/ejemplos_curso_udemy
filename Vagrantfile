Vagrant.require_version ">= 1.7.0"


Vagrant.configure("2") do |config|
  config.vm.box = "gyptazy/ubuntu22.04-arm64"
  config.ssh.insert_key = false

  config.vm.provision "ansible" do |ansible|
    ansible.verbose = "v"
    ansible.playbook = "playbook.yml"
  end


  config.vm.define "ubuntu01" do |ubuntu01|
    ubuntu01.vm.network :public_network, ip: "192.168.1.150"
  end

  config.vm.define "ubuntu02" do |ubuntu02|
    ubuntu02.vm.network :public_network, ip: "192.168.1.151"
  end

end
