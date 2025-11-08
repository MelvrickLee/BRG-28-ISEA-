# BRG-27-ISEA-

Repo for ISEA Bridging

This file documents my learning reflection



\## added on @ 8/11 : 1242



Session 1a

Obtaining Linux:



Installation process is straightforward, but it seems like default memory allocation for video is insufficient for Ubuntu (will result in black screen with nothing happening). 32mb is needed.



Installation process is slow, maybe increasing CPU will make it go faster?





\## added on @ 8/11 : 1511



CLI Fam:



pressing 1 and q whilst in "top" is the same as navigating a menu and pressing options

ls -la displays more information on ls. But i do not know what the information is presenting as of yet.

The difference between nano and gedit/featherpad is that nano uses CLI whilst the latter uses GUI to edit text. As this is the case, i will not be able to edit the text using gedit if i only have a remote terminal prompt.

cp copies the file whilst mv renames the file

after experimenting, i believe that ls shows me a simplified directory whilst ls -lah shows me when the file was last updated/accessed



uname shows the system information, along with the os version and when it was last updated. lsb\_release looks for lsb\_module and displays the current OS information like version name, current version number and the distributor



ls -alt seems to display when the file was last altered. hostnamectl displays system information that is easily readable to humans.

i am able to ping google, but it keeps pinging multiple things (had to manually close terminal to get back control). it looks like the ping is pinging all routers/servers affiliated with google



lsusb and lspci is telling me the hardware connected on the respective usb and pci slots of my computer. less/proc/cpuinfo tells me the cpu infomation and its specs. as expected, the computer only have 1 core as that is how many cores i set for the virtual machine.



Although the CLI method to gets more infomation is more useful for troubleshooting/debugging, i prefer the GUI as its easier to comprehend the infomation i need daily



lsusb < out\_of\_lsusb seems be to creating a new file called the latter, with infomation from lsusb being the data to be written.



less displays the file in a new command window that can be returned with q. cat simply prints the data inside the file to the terminal



i think the file is 181 bytes

as the directory has changed, it might have a different output. but the command  less /etc/apt/sources.list.d/ubuntu.sources displays the digital certificate of repositories (who signed them and the uri from where its from). however, it doesnt seem to include apps downloaded from outside the app store.



sudo apt update seems to check if any apps/modules have any updates available. it does not install the updates



the source code is different from machine code as machine code is saved as a binary file (1 and 0) and thus unreadable to humans. source code is written in syntaxes that is understandable by humans, and it thus readable. this happens as compilation turns the readable syntaxes into sets of instructions, and translate it to 1 and 0



SAAS is the easiest to install as you only require a valid account. however, it does require the service provider to be running and you need to have a stable connection to the internet



downloading from a repository is the easiest for the user, as installation is executed at a click of a button. however, the user may not be able to find the app they want if its not in the repository and need to find and add a repository that has it. they would also need an internet connection to install an app



installing from source code is the most secure and reliable method as the user does not need internet connection to download anything, and the user can verify what the code does before installing (assuming they did read the code). however, it is the most cumbersome method as it requires one to have the source code, and ensure the code compiles properly. the installed app also does not automatically update unlike in SAAS and downloading from repository. thus the the user needs to undergo the same process with the updated source code to make any updates.

