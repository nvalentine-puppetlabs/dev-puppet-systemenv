# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure('2') do |config|
#  config.vm.box = 'ubuntu-12.10-amd64-server'
#  config.vm.box = 'debian-6.07-x86_64'
  config.vm.box = 'centos-6.4-x86_64-cm'
  config.vm.provision :puppet do |p|
    p.manifests_path = 'puppet/manifests'
    p.module_path = 'puppet/modules'
    p.manifest_file = 'site.pp'
    p.options = '--verbose'
  end 
end
