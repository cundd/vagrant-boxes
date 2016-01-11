# vagrant-boxes
Collection of handcrafted Vagrant Boxes

## Usage

Import the box
```bash
vagrant box add dupal https://github.com/cundd/vagrant-boxes/releases/download/0.1.0/alpine-3.3.0-x86_64.box
vagrant init dupal;
vagrant up;
```

Configure a private network with a fixed IP address and use NFS for shared directories
```ruby
config.vm.network "private_network", ip: "192.168.33.10"
config.vm.synced_folder ".", "/vagrant", type: "nfs"
```
