# Rails Vagrantfile

Vagrantfile for Ruby on Rails (RoR) Applications

This is intended to be minimally invasive to the host machine, and has no dependencies other than [Vagrant](http://www.vagrantup.com/) itself.

## Setting Up a Ruby On Rails VM

Install [Vagrant](http://www.vagrantup.com/).

Download the Vagrantfile [here](https://raw.githubusercontent.com/olliebennett/rails-vagrantfile/master/Vagrantfile), or clone this repo.

	git clone https://github.com/olliebennett/rails-vagrantfile.git

Boot up (and provision) the virtual machine.

	vagrant up

SSH into the VM:

	vagrant ssh

Open the shared folder (from within the SSH session)

	cd /vagrant

Create a new application (if you don't have one already)

	rails new app_name

Bundle an (existing) application (to install dependencies)

	bundle

Run Ruby on Rails!

	rails server

## Notes

This Vagrantfile is for creating RoR applications, not for use when developing Ruby on Rails itself (unlike [`rails/rails-dev-box`](https://github.com/rails/rails-dev-box)).