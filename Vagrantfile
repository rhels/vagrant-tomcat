Vagrant.configure(2) do |config|
  config.vm.box = "precise32"
  config.vm.box_url = "http://files.vagrantup.com/precise32.box"
  config.vm.network :public_network
  config.vm.network "forwarded_port", guest: 8080, host: 80
  config.vm.provision :shell, :path => "tomcat.sh"
end
