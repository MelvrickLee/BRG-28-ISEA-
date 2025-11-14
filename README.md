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



as the directory has changed, it might have a different output. but the command  less /etc/apt/sources.list.d/ubuntu.sources displays the digital certificate of repositories installed (who signed them and the uri from where its from).



sudo apt update seems to check if any apps/modules have any updates available. it does not install the updates



the source code is different from machine code as machine code is saved as a binary file (1 and 0) and thus unreadable to humans. source code is written in syntaxes that is understandable by humans, and it thus readable. this happens as compilation turns the readable syntaxes into sets of instructions, and translate it to 1 and 0



SAAS is the easiest to install as you only require a valid account. however, it does require the service provider to be running and you need to have a stable connection to the internet



downloading from a repository is the easiest for the user, as installation is executed at a click of a button. however, the user may not be able to find the app they want if its not in the repository and need to find and add a repository that has it. they would also need an internet connection to install an app



installing from source code is the most secure and reliable method as the user does not need internet connection to download anything, and the user can verify what the code does before installing (assuming they did read the code). however, it is the most cumbersome method as it requires one to have the source code, and ensure the code compiles properly. the installed app also does not automatically update unlike in SAAS and downloading from repository. thus the the user needs to undergo the same process with the updated source code to make any updates.



\## added @ 9/11 : 1557

session 1b



Linux Services:



it seems like http://127.0.0.1 is the default address for everyone despite everyone having a different IP/MAC address



upon using nano, i was notified that the file was unwritable. maybe i could use SUDO to override the perms



the only difference between gedit and nano is gedit opens the file into a text editor, whilst nano prints the text in the CLI





nmap seem to show me that port 80 is open, using the tcp protocol and running http service.



after removing apache2, the entered ip address in nmap does not show the network protocol, network application protocol or service (does not show http, tcp and the port that is open)



the change is probably because the targeted ip is no longer expecting any network request/connection as its no longer a server. 



sudo is needed as changing firewall settings needs admin permissions



after enabling a firewall, i was unable to scan the computer ports, or even ping it.





after adding the firewall rule, i was able to ping the computer. however on the the nmap output, instead of telling me the other 999 ports are closed, it says that they are filtered. it also says that they is no response from them instead of being refused connection (this is under the "not shown" section.



upon entering the code, nothing seems to happen and the terminal breaks (no response, prompts or anything). my best guess is because there is a user logged in already, or there are no user login information the system can use. 



upon further investigation, this might have something to do with the firewall, and i was able to have remote access to the console, but i needed the password for the default user (asked me for password for one user only, which is the default).



if ssh uses a specific port, i can selectively open a port for it by adding a rule to the firewall





in the /etc/passwd directory, it looks like a list of services, protocols, users or folders, with their directory and if they need login information to be accessed



the new account was added, and the default address/number is the previous account + 1. also seems like the information was stored in the /home folder











\## added @ 9/11 : 1519

session 2a





TCO:



Company:



Assuming company “A” uses paper prints for supporting documents in business meetings and meeting notes. Assumed 140 pages are printed a week. No scanning of documents will be done. The printer is expected to be used for a minimum of 5 years and will be left idle from Monday to Friday, 8:00 am to 6:00 pm (50 hours in total). Assume even use of all colours during coloured prints, and black is used 3x more than CMY.



Consumables used (a year):

6850 sheets of paper (assume all single-sided prints)

2350 hrs left on/powered (940hrs active, 1410 hrs idle)



Printers:

MFC-J3940DW Inkjet Printer ($718)

HP Color LaserJet Pro MFP 3303fdw Printer ($599)

HL-L3240CDW Laser Printer ($368)

HL-L3230CDN Laser Printer ($358)







specs

MFC-J3940DW Inkjet Printer ($718):

3k pages for black ($54/cartridge)

1.5k pages for colour (CMY, $92/pack)

2 black cartridges, 1 colored refill a year

5.5W active, 0.9W idle, 0.03W Off

28IPM prints

500 sheets capacity

Prints up to A3

Inkjet printer

Have scan and fax



HP Color LaserJet Pro MFP 3303fdw Printer ($599)

3.2k pages for black ($144/cartridge)

2.5k pages for colour ($165.40/cartridge)

2 black cartridges refill a year, one coloured refill every other year

416W printing, 7.6W ready, 0.95W idle, 0.05W off

25 PPM

500 sheets capacity

Up to A4 prints

LaserJet Printer

Have scan and fax



HL-L3240CDW Laser Printer

3k pages, black ($117/catridge)

2.3k Pages, coloured ($138/catridge, CMY)

2 black refills a year, 1 colour refill every 2 years

Don’t need to refill drum ($200, 50k pages refill if needed)

70W printing, 10W idle, 0.04W off

Relatively quiet

Up to A4 prints

250 sheet capacity

26PPM



HL-L3230CDN Laser Printer

3k pages black ($121/catridge)

2,3k pages, coloured ($143/catridge, CMY)

2 black refills a year, 1 coloured every 2 years

1 refill of drum is needed for 5 years ($221, 18k pages)

75W printing, 8.8W idle, 0.04W off

250 sheet capacity

Up to A4 Prints

18PPM





Power cost (in order)

940h printing, 1410h idle/ready(HP), 6410h off

5170, 1269, 192.3 : $1991.38

391040, 1672, 320.5 : $118,027.66

68500, 14100, 256.4 : $24,881.78

70500, 12408, 256.4 : 24,974.27



Paper cost:

Total paper use = 34250 = 68.5 REAMS

Assuming company has a contract with PaperOne for 70g paper

100 REAMS at 3.45/REAM = $345

Used = ~$236.33



TCO (in order):

718 + 1000 + 236.33 + 1991.38 = $3,945.71

599 + 3921 + 118027.66 + 236.33 = $122,783.33

368 + 2412 + 24881.78 + 236.33 = $27,898.11

358 + 24974.27 + 2,497 + 236.33 = $28,065.6

\*this is before adding maintenance/repairs, which can be up to around 10-20% of TCO, as well as accounting for inflation



Conclusion:

For Company “A”, the HL-L3240CDW Laser Printer is the best printer for them as it has the lowest TCO.







Reflection:

If the printer was for home user that prints 5 pages a day, the best printer (for TCO) changes. However, if I were to choose from the 4 options I gave, it would be the HL-L3230CDN Laser Printer, as it is cheaper to purchase as although it has a higher TCO for a company, it would be significantly lower for a home user as significantly lesser prints is done and the user can unplug the printer from the power outlet when not in use.



Apart from TCO, the printer’s capability, compatibility and upfront cost also needs to be taken into consideration when choosing. If the company was an arts company that prints artwork, than the MFC-J3940DW Inkjet Printer would have been the better choice as it is an InkJet printer.



For a large workgroup, the ideal printer would have a high PPM count, high sheet capacity and good reliability as we want to reduce the time wasted on waiting for a printer to finish it’s task, time used to refill the paper tray and resources spent/hours wasted on repairs



Assuming that the chosen printers don’t break down, the TCO gap between all of them will remain the same. However, the only time the TCO will the same is if one printer keeps breaking down and require maintenance/repairs.





\# added @ 9/11 : 1528

session 2b



AWS:



As i do not have a credit card, i cannot sign up for AWS, so i will begin from launching apache from the virtual machine and using that as my server





BASH:





mkdir was used to make a new directory.



cat command can be used to view file contents without opening a GUI (prints content into CLI). nano can also be used (allows for editing content as well)



cp is copy the contents of a file into a new file, and save it under a new name. mv renames the file (does not create a new file)



chmod tells the system to change the file permission/type. we didn't use +x, but upon research, 777 gives the file read/write permissions for all users. +x makes the file into an executable usable for specified users if the user group is specified, else it gives it to everyone.



shebang is probably used at the beginning of script to indicate a bash script



my modifying the echo command, i can change the contents of the message. if its to print a message that has variable output, than using a $ infront of the variable. this indicates to the program to print the value and not the name of the variable

