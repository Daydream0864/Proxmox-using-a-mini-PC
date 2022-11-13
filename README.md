# Proxmox-using-a-mini-PC

## Why I converted a mini pc
I converted a mini pc because of coururosety and fun at experimenting.
having a homelab where you can test something out and if the system crashes just reset or make new one.
proxmox can be used for many things. creating Virtuel machines, storage server, Docker images, etc.
Mini pc's are relatively cheap and perfect for that.

* MINIS FORUM
* M.2 2280 512 GB PCIe SSD
* Intel Core i5-8279U Prozessor, 4 cores / 8 Threads (6M Cache, - 4,10 GHz)
* Intel Iris Plus Graphics 655 (300 MHz - 1,15 GHz)
* 16GB DDR4
* DC 19V
* 16 x 15.8 x 10.6 cm

# Conversion

## Flashing the USB
the first step is to flash the Proxmox ISO image to a USB drive.
software:
 * https://rufus.ie/en/
 * https://www.balena.io/etcher 
 
ISO image from the website :
 * https://www.proxmox.com/en/
 
## BIOS and install Proxmox

First is the temporary set up a monitor and a keyboard and mouse. plug in the USB drive in to the Computer. plug in the LAN-cable that is connected to the router. To get in the BIOS is spamming the DEL key.
In the BIOS the only thing need to change is in the security settings disable 'safe boot' option, or 'secure boot'. after that restart and spamm the F7 key for the Boot device manager.
select the USB drive and it will pop up the Proxmox install guide.

## proxmox install guide

the guide is simple just follow the instruction. for the IP chose one that is free.(for more info https://www.howtogeek.com/341307/how-do-ip-addresses-work/)
 
after everthing is done the proxmox Terminal will appear with the 'https' adress and write it down, but before that log in the terminal and use 'sudo apt update'and
'sudo apt upgrade' after that use the linux "shutdown" command. unplug the USB drive and monitor,keyboard and mouse. place the mini next to your router or somewhere. start the mini PC and use your main set up (main PC) for further use.

## Proxmox web-GUI

open a web browser and write the 'Https' address into your search bar. welcome to proxmox it is possible to interact with the mini pc/ server.
here are some other install tutorials:
* https://www.youtube.com/watch?v=_u8qTN3cCnQ
* https://www.youtube.com/watch?v=azORbxrItOo



### tips
* dont delete the lvm storage. use it for the VM storage.
* remote desktop via rustdesk or Remmina, or usind SPICE proxmox. and many other options.( I use rustdesk)

# Thanks for reading


 
 
 



