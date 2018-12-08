Vagrant.configure("2") do |config|
  config.vm.box = 'adpe/centos-neos'
  config.vm.box_version = "0.1"
  config.vm.hostname = 'neos.local'
    
  config.hostmanager.enabled = true
  config.hostmanager.manage_host = true
  
  config.vm.network 'private_network', ip: '10.0.3.11'
  config.ssh.forward_agent = true

  config.vm.synced_folder ".", "/vagrant", create: true, type: "nfs"
  
  config.vm.provider 'virtualbox' do |vb|
    vb.name = 'neos.local'
    vb.gui = false
    vb.memory = '2048'
    vb.cpus = 1
  end
end
