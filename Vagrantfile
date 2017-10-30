Vagrant.configure(2) do |config|

  config.ssh.insert_key = false

  # CentOS 6
  config.vm.define "lab-1" do |node|
    node.vm.box = "samdoran/centos6"
    node.vm.hostname = "lab-1"
    node.vm.network "private_network", ip: "10.77.1.31"

    node.vm.provider :virtualbox do |vbox|
      vbox.name = "lab-1"
      vbox.memory = 256
      vbox.cpus = 1
    end

  end

  # CentOS 7
  config.vm.define "lab-2" do |node|
    node.vm.box = "samdoran/centos7"
    node.vm.hostname = "lab-2"
    node.vm.network "private_network", ip: "10.77.1.32"

    node.vm.provider :virtualbox do |vbox|
      vbox.name = "lab-2"
      vbox.memory = 512
      vbox.cpus = 1
    end

  end

  # Debian7/Wheezy
  config.vm.define "lab-3" do |node|
    node.vm.box = "debian/wheezy64"
    node.vm.hostname = "lab-3"
    node.vm.network "private_network", ip: "10.77.1.38"

    node.vm.provider :virtualbox do |vbox|
      vbox.name = "lab-3"
    end

  end

  # Debian8/Jesse
  config.vm.define "lab-4" do |node|
    node.vm.box = "debian/jessie64"
    node.vm.hostname = 'lab-4'
    node.vm.network "private_network", ip: "10.77.1.39"

    node.vm.provider :virtualbox do |vbox|
      vbox.name = "lab-4"
    end

  end

end
