$script = <<-SCRIPT
which aws &>/dev/null || {
  which pip3 || {
    sudo apt-get update
    sudo apt-get install -y python3-pip
  }

  pip3 install --upgrade awscli

}
SCRIPT

Vagrant.configure("2") do |config|
  config.vm.box = "alvaro/bionic64"
  config.vm.provision "shell", inline: $script, privileged: false
end

