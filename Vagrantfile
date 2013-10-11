# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant::Config.run do |config|
  # Every Vagrant virtual environment requires a box to build off of.
  config.vm.box = "precise64"

  # The url from where the 'config.vm.box' box will be fetched if it
  # doesn't already exist on the user's system.
  config.vm.box_url = "http://dl.dropbox.com/u/1537815/precise64.box"

  # This will execute the following scripts in the shell of the newly created VM.
  config.vm.provision :shell, :path => "scripts/deploy.sh"

  # So graphical programs may be used from the VM
  config.ssh.forward_x11 = true

end
