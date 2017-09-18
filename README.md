# Ansible Vagrant JupyterHub

This repository contains different virtual machines having different setups for providing Jupyterhub setup with nbgrader. The virtual machines are created by Vagrant and provisioned by Ansible.

Each directory has a different setup of JupyterHub. To use a particualr setup do the following:
1. Install the following dependecies as per your machine (Linux, Windows or Mac) 
	* [Vagrant](https://www.vagrantup.com/downloads.html)
	* [Virtual Box](https://www.virtualbox.org/)
	* [Ansible](http://docs.ansible.com/ansible/latest/intro_installation.html)	

2. Clone the repository.
3. Change directory into 1 of the examples.
4. run ``` vagrant up ```  This will bringup a virtual machine with debian and all the required packages will be installed.
5. Now in your host machine you can go to a browser ``` https://192.168.50.10``` , to login to the Juypterhub (login and credintials please read the README.md in each of the folder)
6. Shutting down `$> vagrant halt`

# License

Mozilla Public License 2.0 

# Acknowledgements

1. [JupyterHub deploy teaching ](https://github.com/jupyterhub/jupyterhub-deploy-teaching)
2. [Vagrant Ansible examples](https://github.com/geerlingguy/ansible-vagrant-examples)
