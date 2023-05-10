# osc23_Podman_Containers_with_Ansible_Nginx

Vagrant setup to demonstrate setting up a nginx container, running with Podman
and systemd, by using Ansible.

## Requirements

Vagrant-libvirt. Ansible. Git. Fun.

## Usage

1. Checkout this repository.
2. Make sure that all git submodules are up to date by running `git submodule
   init && git submodule update`
3. Fetch the vagrant box: `vagrant box add opensuse/Leap-15.4.x86_64`
4. Run `vagrant up`.
5. Connect to your VM's IP address using the right port (see below).
6. You should see a web page.
7. Party!

The `main` branch contains all things necessary to run a `rootless` container.
In this case, the nginx container is listening on port 8080.

The `rootful_container` branch sets up a container running as a systemd system
service. It is listening on port 80.

## License

BSD-3-Clause

## Author Information

I am Johannes Kastl, reachable via kastl@b1-systems.de.
