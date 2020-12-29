Vagrant.configure("2") do |config|
  config.vm.box = "centos/8"
  config.vm.provision "file", source: "~/.ssh/id_rsa.pub", destination: "~/.ssh/me.pub"
  config.vm.provision "shell", inline: <<-SHELL
      cat /home/vagrant/.ssh/me.pub >> /home/vagrant/.ssh/authorized_keys
    SHELL
  config.vm.network "public_network", ip: "192.168.0.177"
end
