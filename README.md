# Server_Setup
This script will help install any, or all, of Docker-CE, Docker-Compose, NGinX Proxy Manager, and Portainer-CE.

Reason for Making this Script
I got tired of running individual commands all the time, so I created some scripts to make this very easy.

Using this script

Clone the repo
git clone https://gitlab.com/bmcgonag/docker_installs.git


, or copy / paste the code from the install_docker_nproxyman.sh file into a file on your server.
nano docker-install.sh
to open a text editor in the terminal, then use CTRL + Shift + V to paste into it.
Save with CTRL + O, then Enter to confirm, and exit the nano editor with CTRL + X.

Change the permissions of the .sh file to make it executable with.

chmod +x docker-install.sh

Run the installer with

./docker-install.sh

Prompts from the script:
First, you'll be prompted to select the number for your OS / Distro.  Currently I support CentOS 7 and 8, Debian 10 and 11, Ubuntu 18.04, 20.04, 22.04, Arch Linux, and Open Suse (tested on Leap 15.4).
Next, you'll be asked to answer "y" to any of the four software packages you'd like to install.

Docker-CE
Docker-Compose
NGinx Proxy Manager
Navidrome (music player))
Portainer-CE

if you answer y to Portainer, you'll be asked another question



Do you want

full Portainer-CE with the web UI, or
just Portainer-agent (which you connect to another full portainer instance).

Make that selection, and the install will continue.
Answering "n" to any of them will cause them to be skipped.

NOTE

You must have Docker-CE (or some version of Docker) installed in order to run any of the other three packages.
You must have Docker-Compose installed in order to run NGinX Proxy Manager, Portainer-CE, or Navidrome with this script.

Before prompting to install Docker or Docker-Compose, I do try to see if you already have them installed, and I skip the prompt if you do (or I try to anyway).

# Credit
https://gitlab.com/bmcgonag/docker_installs/-/tree/main/
