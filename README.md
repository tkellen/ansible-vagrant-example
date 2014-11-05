# vagrant-ansible
> A super simple example.

## Setup

Install the following:

- VirtualBox ([download](https://www.virtualbox.org/))
- Vagrant ([download](http://www.vagrantup.com/downloads.html))
- Ansible
  - `pip install ansible` via [pip](http://pip.readthedocs.org/en/latest/installing.html) (All Platforms)
  - `brew intall ansible` via [homebrew](http://brew.sh/) (OSX)
  - `apt-get/yum install ansible` (Linux)

Then run `vagrant up`.


### FAQ

#### Vagrant threw an error about ssh/ansible during `vagrant up`
This happens occasionally when Ansible tries to provision the box before the network interface is initialized. Try running `vagrant provision` manually after `vagrant up` completes.
