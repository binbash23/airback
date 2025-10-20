# airback

Written by
	Jens Heine <binbash@gmx.net>
	Dennis Brossat <dennis.brossat@email.de>
	Benjamin Heine <benjaminheine@gmx.net>

Do you want to backup the pictures and videos from your android mobile to your linux server (or any windows system with ssh)?
Use airback and it will start backing up your data when your mobile appears in your wifi network.


HOWTO

Dependencies

First install this tools on your client system (PC):
 nmap
 fusermount
 sshfs
 nice


Then install a ssh server on your mobile. I recommend using [termux](https://play.google.com/store/apps/details?id=com.termux&hl=de) .
To install and grant access to the android filesystem you can follow these steps:

- install termux on the mobile an start a session
- Update termux: "pkg upgrade"
- Install ssh: "pkg install openssh"
- Grant filesystem access to termux: "termux-setup-storage"
- Connect from your PC to the mobile with ssh 
- If you do not want to type the password everytime, I recommend to enable ssh key authentication (i.e. ssh-copy-id)

Download airback and copy it to a folder in your path.
Run airback:

"airback -h" for help
or
"airback" to run it. A config file will be created.

Please send feedback
Good luck, Jens
