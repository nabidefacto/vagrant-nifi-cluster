# vagrant-nifi-cluster

Local nifi cluster with vagrant provisioning 

It's required to put nifi archive file (for example  nifi-1.0.1-bin.tar.gz) where Vagrantfile located.

After vagrant up wait for 5-10 minutes and we will have NiFi cluster with 3 nodes.

if it staring slow, remove this line in Vagrantfile:
srv.vm.provision :shell, inline: "/opt/nifi-1.0.1/bin/nifi.sh start"
