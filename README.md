# Content of this repo

## Vagrant

For the config of the environment, I used the guide in (I)
The vagrant file just creates a couple of Ubuntu VMs.
For the deployment of those VMs, I needed a provider that works on Apple arm64 architecture. Therefore I had to use VMware Fusion with a license for personal use.
For the integration of Vagrant and the VMWare Fusion with the plugin, I used the software package vagrant-vmware-utility_1.0.22_darwin_amd64.dmg

```
angelito@Mac-mini-de-Angel /Users/angelito/repos/ansible/ejemplos_curso_udemy                                                                                                                                                                                          main
⚡ vagrant plugin list
vagrant-share (2.0.0, global)
vagrant-vmware-desktop (3.0.3, global)
```

## Ansible for lab provisioning

Creates an user called ansible and adds a testing SSH key, not included in the repo.

## Inventory of the lab

Defines the two VMs for playing

## References

- I: https://www.unixarena.com/2022/09/virtual-machine-on-apple-mac-chip-m1-m2-fusion-vagrant.html/
- II: vagrant-vmware-utility_1.0.22_darwin_amd64.dmg

## Needs to be fixed

Enable ansible user to escalate as root for being able to use --become
