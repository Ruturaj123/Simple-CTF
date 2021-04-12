This is a project that I developed for the course [COMPSCI 590A](https://infosec.cs.umass.edu/content/compsci-590a-system-defense-and-test). It is a simple Capture the flag, which uses Kali-Linux as the attack machine and Ubuntu as the target.

## INSTRUCTIONS
This CTF consists of 3 levels. The first level is very easy and should be completed on Ubuntu itself. Whereas the next 2 levels should be completed via the attack machine (Kali-Linux). Please do not open any other folders of this repository, apart from level_1, as this may spoil the fun of the challenge :) <br>
Also, there are three separate files which contain hints for these levels. You can use them if you feel stuck at any point. <br>
At every stage, save the flag that you get because you will need it in the end.

### How to run?
1. Start up Kali-Linux and Ubuntu in two separate windows via VirtualBox (or VMWare).
2. Install [docker](https://docs.docker.com/engine/install/ubuntu/) and [docker-compose](https://docs.docker.com/compose/install/#install-compose-on-linux-systems) on the Ubuntu VM.
3. Clone this repository on the Ubuntu VM
4. Enter the following command on the Ubuntu VM, from the root directory of this folder:
```sh
$ docker-compose up -d
```

It may take several minutes to start, as docker will download the necessary modules for setting everything up.

## Level 1:
Open a folder called level_1 on the Ubuntu VM, you may find your first flag there!

## Level 2:
The second flag is inside one of the docker containers, the challenge is to get access to this container via the attack machine.


## Level 3:
The mysql username is one of the most famous usernames & the password is a permutation of the string "ctf590a"


Finally, combine the 3 flags that you got, and it will become the password of the final.zip file. Extract this zip file using the combined password to complete the challenge!
