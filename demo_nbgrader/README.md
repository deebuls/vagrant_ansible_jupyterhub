# Vagrant Ansible for Jupyterhub + nbgrader demo

## Background

This setup provides a virtual machine using Virtualbox with JupyterHub and nbgrader installed.

## Steps
This README file is inside a folder that contains a `Vagrantfile` (hereafter this folder shall be called the [vagrant_root]), which tells Vagrant how to set up your virtual machine in VirtualBox.

To use the vagrant file, you will need to have done the following:

  1. Download and Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
  2. Download and Install [Vagrant](https://www.vagrantup.com/downloads.html)
  3. Install [Ansible](http://ansibleworks.com/) ([guide for installing Ansible](http://docs.ansible.com/intro_installation.html))
  4. Open a shell prompt (Terminal app on a Mac) and cd into the folder containing the `Vagrantfile`
  5. Run the following command to install `vagrant up`, and Vagrant will create a new VM, install the base box, and configure it.
  6. This will take around 15 - 20 minutes to complete the installation
  7. Once completed, from your *host machine* browser type `https://192.168.50.10` , You should see the login page for jupyterhub

## User informatin
- username: admin, password: admin
  * can add more users in the jupyterhub
  * can create assignments and release them
  * can grade assignments
  * access released assigments and submit
- username: grader, password: grader
  * can grade assisgnments
  * access released assigments and submit
- username: student, password: student
  * access released assigments and submit


## nbgrader 

- After login as admin you can see the *Formgrader* tab.
- Clicking on it will end up on a new page.
- This page has instuctions tab to generate and release assignment through the interface.
- For creating an assignment dont forget to add the nbgrader tags(question/answer/grades) in ipython notebook *(view -> cell toolbar -> create assignmnet)*

## Shuting down
- `vagrant halt`
