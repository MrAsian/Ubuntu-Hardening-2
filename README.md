# Ubuntu-Hardening-2

This is a script created for use on the Ubuntu image for team 2 of the Wando Cyber Defense Club during CyberPatriot competitions. This script is orginally created in 2016. Ongoing Project.

This is the updated and revised version of [Ubuntu-Hardening-1](https://github.com/MrAsian/Ubuntu-Hardening-1).

Usage
-----

Open the terminal and log into sudo with

```bash
sudo su
```

After logging in, cd to where the script is stored and run

```bash
bash script
```

This will run the script, just follow the instructions in the script from there on.

Things in the script
--------------------

- all

  - Runs every command in the script except for end and sys-update. It will ask the user whether or not they would like to have the system update.

- disable-guest

  - Disables the guest account.

- disable-ipv6

  - Disables the use of ipv6.

- end

  - Terminates the script.

- find-things

  - Find some suspicious programs and file types and prints them to the output file. It is up to the user to decide on what to do with the programs and files. Please note that not all of these programs and files are necessarily bad. It is just a list of possible suspicious programs and files to pay attention to.

    - Targetted programs include:

        apache2, bind9, cain, cracklib, hydra, john, nc, netcat, nginx, nikto, postgrsql, samba, telnet, tftp-server, vsftpd

    - Targetted file types include:

       .jpg, .mp3, .mp4, .png

- firewall

  - Installs and enables the firewall with default settings.

- help

  - Opens the Guide, which is basically this readme.

- misc

  - Sets the permission in some files and opens some files that should be looked at during the CyberPatriot competitions.

- pass-policy

  - Sets the password policy.

    - Password minimum length is 12 characters.

    - Password history is 5.

    - Password retry attempt is 3.

    - Password minimum age is 60 days.

    - Password maximum age is 59 days.

- pass-reset

  - Will prompt the user for a password to be used as a default on all accounts. The default password will be set for all acounts, including the current user.
  
  - Input is hidden. It will prompt the user to reenter the password to make sure it is typed correctly.

- secure-root

  - Locks the root account.

- security

  - Install a bunch of security softwares. However, only chkrootkit and bastille will be automatically ran.

    - The list includes:

        apparmor, bastille, chkrootkit, clamav, lynis, rkhunter

- ssh-conf

  - Configures the SSH service.

  - Root account will no longer be able to be logged onto from SSH and SSH will be set to port 222.

- sys-update

  - Performs a system update.

Future Additions
----------------

- Nothing as of right now. Will add more things when it pops into my head.

Contributors
------------
@MrAsian @DrDavid52
