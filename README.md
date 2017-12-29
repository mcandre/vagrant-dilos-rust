# vagrant-dilos-rust: a Vagrant box for building Rust binaries for Solaris/Illumos (DilOS)

# DISCLAIMER

I currently don't see a (straightforward) way to actually install Rust in DilOS. For now, mcandre/vagrant-dilos-rust is simply broken, pending either rustup support for the SunOS/Solaris/Illumos kernel, or else some rare contributor uploading a "rust" package for DilOS. For my purposes, I just want to install the rustc and cargo tools into SOME modern SunOS/Solaris/Illumos virtual machine, in order to build Rust applications targeting the SunOS/Solaris/Illumos kernel. Effort on that front will likely continue in a mcandre/vagrant-smartos-rust box.

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
