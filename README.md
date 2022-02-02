# linux-solutions
This document is the record of linux terminal commands at a useful time to solve bugs or even to help with routine tasks


<h1>Creating SuperUser</h1>
At the terminal write:
<br>
   &emsp;<i>sudo passwd root</i>

Terminal will ask your user password
**After, write and rewrite your Superuser's password.

**And then, to acess your supersuser write:
<br>
   &emsp;<i>sudo passwd -u root</i>



<h1>Reset user password</h1>
Firstly have to reboot the system and inicialize by security mode in the grub (pressing esc when it start, it works for me). Then enter in root mode and white in terminal:
<br>
   &emsp;<i>passwd <strong>user*</strong> </i>
<br>
*name of your user
<br>


<h1>Making a script file in executable</h1>
You write at terminal:
<br>
   &emsp;<i>sudo su</i>
<br>
Put your user's password. Then:
<br>
   <i>&emsp;cd /home/user/.yourscriptfile*
  <br>&emsp;chmod +x yourscriptfile*
	<br>&emsp;./yourscriptfile*
</i>
<br>
*This work in the .sh files
<br>


<h1>"apt-get upgrade" erro</h1>
   <i>&emsp;sudo dpkg --configure -a</i>
<br>
At the terminal, you can apply this solution for:
<br>

<i>
E: Could not get lock /var/lib/dpkg/lock-frontend. It is held by process 6846 (unattended-upgr)
N: Be aware that removing the lock file is not a solution and may break your system.
E: Unable to acquire the dpkg frontend lock (/var/lib/dpkg/lock-frontend), is another process using it?
</i>





