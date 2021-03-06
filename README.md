# vagrant-dilos-rust: a Vagrant box for building Rust binaries for Solaris/Illumos (DilOS)

# DISCLAIMER

Currently broken, will likely continue efforts in a mcandre/vagrant-smartos-rust box, as its pkgin repository features rust.

# VAGRANT CLOUD

https://app.vagrantup.com/mcandre/boxes/vagrant-dilos-rust

# EXAMPLE

```console
$ cd test
$ vagrant up
$ vagrant ssh -c "cd /vagrant && rustc hello.rs && ./hello"
...
```

# RUNTIME REQUIREMENTS

* [Vagrant](https://www.vagrantup.com)
* The [VirtualBox](https://www.virtualbox.org) hypervisor provider

## Recommended

* [vagrant-rsync-back](https://github.com/smerrill/vagrant-rsync-back) assists in copying artifacts from the guest to the host

# BUILDTIME REQUIREMENTS

* [Vagrant](https://www.vagrantup.com)
* The [VirtualBox](https://www.virtualbox.org) hypervisor provider
* [make](https://www.gnu.org/software/make/)

# EXPORT

```console
$ make vagrant-dilos-rust.box
```
