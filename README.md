# Virtual_Machine_Mount_point
https://vineetcic.medium.com/how-to-access-folders-on-ubuntu-host-machine-from-an-ubuntu-virtual-machine-in-virtualbox-a020a9dbc5a4
You followed all the steps provided in the above link and got the following output:bash: cd: shared/: Permission denied. No way to use scp
Simply use sudo su command to create, copy and access folders or file on ubuntu virtual machine and ubuntu host machine 

*@*:~$ sudo su
[sudo] password for manager: 
*@*:/home/...# cd shared/
*@*:/home/.../shared# touch file
*@*:/home/.../shared# ls
 file
root@genseqbioGSB:/home/manager/shared# 
The newly created should be accessible in the folder Path (on the host machine) and folder name (on the virtual machine) set in the VM
Kindly do not tick Read only option in the VM settings (Devices > shared Folders)

Good luck!!

Troubleshooting done by Noutin Michoidgni and NAME Pakyendou NAME, TA of Burkina Faso classroom for GSB_Africa 2023. Thank you Jorge Batista da Roacha for the link. 
