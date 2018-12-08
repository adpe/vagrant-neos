# Neos 4.1.8 Vagrant Box

This is a prepacked Vagrant Box which contains following packages:
- CentOS 7.6
- MariaDB 10.3.11
- PHP 7.2.13
- Neos CMS 4.1.8

## Requirements

- VirtualBox
- Vagrant
- Git

_Tested with Vagrant 2.2.2 and VirtualBox 5.2.22_

## Installation

1. Clone repo to your workspace
`git clone https://github.com/adpe/vagrant-neos.git <your-path>/`
2. If desired adapt `Vagrantfile` to your needs
3. Run `vagrant up`
4. Connect to VM with `vagrant ssh`
5. Check if application runs with http://neos.local

## Appendix
### Predefined credentials

|         | username | password         |
|---------|----------|------------------|
| MariaDB | root     | %dbp4ssw0rd%     |
|         | neosuser | %neosdbpassword% |
| Neos    | admin    | %neosPW%         |

### More information

- CentOS originally from Vagrant `centos/7` box.
- SELinux is disabled

