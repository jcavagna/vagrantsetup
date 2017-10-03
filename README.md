# Easy Vagrant setup on OSX

This is a setup for a basic Vagrant box using Ubuntu 14.04 LTS with PHP and MariaDB

## Installation

**OSX** Ensure you have the latest version of Virtual Box and the extension pack installed with this Vagrant box.

Take the contents of this repo and dump it into the root directory of the project you are working on.

## Usage 
Add a name to your **/etc/hosts** to have the IP address located in the vagrant file under **private_network** to set up easy access with your browser.

Ensure you change the **v.name** to your project name so it won't conflict with other projects you may have running.

The default username and password for MariaDB is **root 1234**. This can be modified in the bootstrap.sh file.

Next enter your terminal and navigate to the the root directory for this project and type:

```
vagrant up
```

Congratulations! Once it scrolls through the installation of the box and provisions, you will see a message stating the loading has finished.

When you are done with the box, navigate in terminal back to the root directory of that project and type:

```
vagrant destroy
```

This will shut down and remove the box from your computer. If you had anything saved in the database, it will need to be recreated. If you would rather keep an instance of it but don't want it currently running, type:

```
vagrant halt
```
