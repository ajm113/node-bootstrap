# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "hashicorp/precise64"
  config.vm.network "private_network", ip: "192.168.33.11"
  config.vm.hostname = "nodejs-foundation"
  config.vm.synced_folder ".", "/var/www", :mount_options => ["dmode=777", "fmode=666"]

  # Install node, npm, bower, and gulp.
  config.vm.provision "shell", inline: <<-SHELL
    apt-get update
    apt-get install -y git curl
    curl -sL https://deb.nodesource.com/setup | sudo bash -
    sudo apt-get install -y nodejs
    sudo npm install -g bower
    sudo npm install gulp-cli -g
    sudo npm install gulp -D
  SHELL
end
