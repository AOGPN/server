# AOGPN server

Ansible to provision a Discourse server for the [Australian Open Government Partnership Civil Society Network](https://opengovernment.org.au/).

## Usage

You'll need a file called `ansible_vault_pass.txt` in the root of this repository that contains the right password in order to decrypt secret things like the SSL key.

### Development

To bring up a local Vagrant box using VirtualBox to develop configuration changes:

    vagrant up

Port 4443 is forwarded to the guest's HTTPS web server so you can connect to the Discourse instance locally at:

[https://localhost:4443/](https://localhost:4443/)

It's configured as forum.opengovernment.org.au so when you get things like email you'll need to manually copy the address back to one that will work locally.

### Production

TODO: Instructions for provisioning a server.

## Memory

We're deploying this to a server with 1 GB of RAM so we need to ensure it has 1 GB of swap.
The Vagrant test box included in this repository just has 2 GB of RAM because it's fiddly to increase swap with Vagrant/VirtualBox.
