
Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.network "forwarded_port", guest: 8080, host: 8080
  config.vm.provision :shell, :path => "launching_programs.sh"
  config.vm.box = "beubi/jenkins"
  config.vm.box_version = "0.0.1"
  config.vm.synced_folder "c:/Users/m.shylau/Documents/Vagrant/projects", "/var/www"
end
