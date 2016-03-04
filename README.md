# server
Ansible to provision a Discourse server.

## Memory

We're deploying this to a server with 1 GB of RAM so we need to ensure it has 1 GB of swap.
The Vagrant test box included in this repository just has 2 GB of RAM because it's fiddly to increase swap with Vagrant/VirtualBox
