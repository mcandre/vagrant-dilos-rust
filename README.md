# vagrant-dilos-rust: a Vagrant box for building Rust binaries for Solaris/Illumos (DilOS)

# VAGRANT CLOUD

https://app.vagrantup.com/mcandre/boxes/vagrant-dilos-rust

# EXAMPLE

```console
$ vagrant up
$ vagrant ssh -c "cd /vagrant && rustc hello.rs && ./hello"
...
```

# REQUIREMENTS

* [Vagrant](https://www.vagrantup.com)
* A VM provider, such as [VirtualBox](https://www.virtualbox.org), [VMware](https://www.vmware.com), or [libvirt](https://libvirt.org)

# EXPORT

```console
$ vagrant destroy -f; vagrant up && vagrant package --output vagrant-dilos-rust.box
```
