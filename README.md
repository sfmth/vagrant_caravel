# vagrant_caravel
Install vagrant (Debian 12):
```
$ nalog install vagrant-libvirt libvirt-daemon-system ansible
$ sudo adduser $USER libvirt
```

To run the tools do this:
```
$ git clone https://github.com/sfmth/vagrant_caravel
$ cd vagrant_caravel/caravel-b8efc55/
$ vagrant up
$ vagrant ssh
$ cd $OPENLANE_ROOT
$ make mount
```
and you'll have access to openlane.
to check if intall has been successful you can run:
```
$ ./flow.tcl -design spm -verbose 1
```
