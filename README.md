This document contains the screenshot and output of all lab activities



Session 1a - AM


##########################################################################

Signup for GitHub Account:
<br/>
<br/>

Creating an account + repository:
<img width="1919" height="942" alt="github" src="https://github.com/user-attachments/assets/2a5b4362-f783-40ab-9841-231123065a21" />
Since I had prior experience with GitHub, I had no trouble creating a repository

<br/> 
As Git was not covered, I used GitHub App to clone the repository onto my local machine
<img width="585" height="155" alt="localRepo" src="https://github.com/user-attachments/assets/feaa7830-2d9c-4f18-9a6f-50b3bda0fefc" />

This screenshot shows the folder of the local repository in windows file explorer

*note that ReadmeBackup.md was added in between the screenshots
<br/>
<br/>

##########################################################################

Obtaining Linux on My PC:
<br/>
<br/>

For the virtual machine application, I chose VirtualBox
I also downloaded the ubuntu ISO file
I proceeded with unattended guest installation with default settings. I also allocated more RAM and video Memory in settings 
The user name is VBoxUser
<img width="1279" height="879" alt="loginLinux" src="https://github.com/user-attachments/assets/76388e3a-f7ef-45ad-99d0-f20a504a65f2" />
*Login Page
<br/>
<br/>

<img width="1279" height="882" alt="homepage" src="https://github.com/user-attachments/assets/fab65485-db8e-4a9c-9683-06bf49407184" />
*Homepage
<br/>
<br/>
<br/>
##########################################################################

Familiarity with Ubuntu Linux:

pwd shows me the current directory i am in
<img width="807" height="576" alt="pwd" src="https://github.com/user-attachments/assets/9c46306d-4725-492d-b309-3fab5a54d162" />
<br/>
<br/>

ls shows me all the files that are in my current directory i am working with
<img width="808" height="576" alt="ls" src="https://github.com/user-attachments/assets/7b895323-1557-4657-a7a2-c802f33de731" />

*CLI view
<br/>
<br/>

<img width="571" height="493" alt="lsFiles" src="https://github.com/user-attachments/assets/4551c357-3a83-4408-bcdb-edd778b7cc17" />

*GUI view (files explorer)
<br/>
<br/>

cd changes my working directory to another folder in the current directory i am on. if i want to work on Documents instead of home, i would use cd Document (note it is case sensitive)
<img width="813" height="571" alt="cd" src="https://github.com/user-attachments/assets/45c07bab-842b-49fe-8432-53182a3273ec" />

*CLI view
<br/>
<br/>

<img width="572" height="492" alt="documents" src="https://github.com/user-attachments/assets/ac118411-672f-4148-8709-37ebecd02097" />

*contents of "Documents"
<br/>
<br/>

mkdir makes a folder inside the working directory i am in. I can also specify the file name. Following from the cd command, I will create a folder named "ISEA" and change directory to there
<img width="812" height="575" alt="mkdir" src="https://github.com/user-attachments/assets/e76ba517-6ca1-49bd-9311-184a52e2ddd7" />

*CLI view
<br/>
<br/>

<img width="572" height="490" alt="mkdirGUI" src="https://github.com/user-attachments/assets/c897a766-aa0c-4d70-a862-628c0873d2c1" />

*Files view
<br/>
<br/>

touch creates an empty file inside the working directory. i can define the name and file extension.
<img width="814" height="576" alt="touch" src="https://github.com/user-attachments/assets/85f187db-7592-4363-9e4d-e49003e80147" />

*CLI View
<br/>
<br/>

<img width="575" height="492" alt="touchGUI" src="https://github.com/user-attachments/assets/3ec1dc0f-0df0-43b2-8d55-33a3091d3e26" />

*Files view
<br/>
<br/>

Exploring Man (or linux console manual)
<img width="920" height="572" alt="man" src="https://github.com/user-attachments/assets/6a95cdf3-6ec2-4b4c-8e19-b1e864c50749" />

*1st page of manual, too many pages in total to document
<br/>
<br/>

##########################################################################
<br/>
<br/>

Session 1b - PM
<br/>
<br/>

##########################################################################

Linux Services:
<br/>
<br/>

"systemctl list-units --type=service" lists all services installed
<img width="1202" height="576" alt="services" src="https://github.com/user-attachments/assets/d4874603-e3c2-402f-8fba-96fb345d6322" />

*1st page of services
<br/>
<br/>

<img width="1203" height="577" alt="servicesEnd" src="https://github.com/user-attachments/assets/f2261781-8f9b-4f55-a44f-82c7788d2447" />

*last page of services

page can be navigated using arrow keys
<br/>
<br/>

to test start/stopping services with CLI, i will be using the UFW service as an example

before command
<img width="1084" height="572" alt="ufwb4" src="https://github.com/user-attachments/assets/4ec233c3-0a94-4e12-b58f-79ef7009e9c6" />


*highlighted is UFW
<br/>
<br/>

after command
<img width="1084" height="574" alt="ufwAfter" src="https://github.com/user-attachments/assets/e72ac493-9ef7-491a-a6b4-18216d29203a" />



*note that number of total active services went down and UFW cannot be found
<br/>
<br/> 

checking service status using systemctl status (using UFW as example)

if service is on
<img width="972" height="576" alt="UfwOn" src="https://github.com/user-attachments/assets/f657cb3a-4866-4d6c-96c4-c67466725b4b" />

<br/> 
<br/> 

if service is off
<img width="979" height="583" alt="UfwOff" src="https://github.com/user-attachments/assets/4a663a69-a819-4dec-953c-17fe0dd42155" />
<br/> 
<br/> 


Linux Permissions:

output for ls -l 

<img width="808" height="574" alt="permissions" src="https://github.com/user-attachments/assets/a614eb84-7ec7-482e-8ba6-9bd9ff2de027" />

*r means read, w means write and x means execute. the 1st column is for onwer, 2nd for group and 3rd for others. d denotes that the file is a directory
<br/>
<br/>

changing permissions (changing testfile to rw -r -r)
<img width="815" height="574" alt="chmod" src="https://github.com/user-attachments/assets/471cc3bd-2133-4120-98c6-05a1762e10dd" />


*highlighted is testfile
<br/>
<br/>

changing ownership of file (from Vboxuser > test)

new account (test)

<img width="1275" height="870" alt="NewUser" src="https://github.com/user-attachments/assets/fef5fb34-5e97-4523-ac86-3fcec73a1a7f" />

<br/>
<br/>
before changing owner
<br/>
<img width="808" height="574" alt="permissions" src="https://github.com/user-attachments/assets/304021df-ebf4-4ab7-a047-2f8478f0048c" />
<br/>
<br/>

after changing owner

<img width="817" height="575" alt="chown" src="https://github.com/user-attachments/assets/240b1e13-d40c-4dd6-b527-4d5e86992c33" />

*note that the testfile (highlighted) changed from vboxuser to test in the 1st row of names
<br/>
<br/>

Searching Filesystems:

for this lab, ill be using findme.txt
<img width="813" height="576" alt="findmeFile" src="https://github.com/user-attachments/assets/dd0506b6-ce99-457d-a05d-ac4e2cb70b62" />


*file location
<br/>
<br/>

the contents of the file

<img width="815" height="571" alt="findmeContent" src="https://github.com/user-attachments/assets/2c9a3c7b-04b5-4889-9999-4027ae14d027" />
<br/>
<br/>

using find from home directory
<img width="814" height="577" alt="findOutput" src="https://github.com/user-attachments/assets/5d080a2b-3a81-41ea-b707-068c4ed5585d" />

*if searching specifically for this file, name must include name + extension. 
**searching just for extension will show all files with said extension
<br/>
<br/>

using grep

<img width="817" height="588" alt="grepOutput" src="https://github.com/user-attachments/assets/0e07255b-1caa-4f46-8861-594149db47af" />

*grep prints the line where the search word is found, but highlights the search word
<br/>
<br/>

##########################################################################
<br/>
<br/>

Session 2a - AM
<br/>
<br/>
##########################################################################

TCO:

*the following content is for calculating TCO instead of cloud providers since during the class time, we were told to do calculations on TCO for printers
<br/>
<br/>

Company:
Assuming company “A” uses paper prints for supporting documents in business meetings and meeting notes. Assumed 140 pages are printed a week. No scanning of documents will be done. The printer is expected to be used for a minimum of 5 years and will be left idle from Monday to Friday, 8:00 am to 6:00 pm (50 hours in total). Assume even use of all colours during coloured prints, and black is used 3x more than CMY.
<br/>
<br/>

Consumables used (a year):
6850 sheets of paper (assume all single-sided prints)
2350 hrs left on/powered (940hrs active, 1410 hrs idle)
<br/>
<br/>

Printers:
<br/>

MFC-J3940DW Inkjet Printer ($718)
HP Color LaserJet Pro MFP 3303fdw Printer ($599)
HL-L3240CDW Laser Printer ($368)
HL-L3230CDN Laser Printer ($358)
<br/>
<br/>

specs:

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
<br/>
<br/>

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
<br/>
<br/>

HL-L3240CDW Laser Printer ($368)
3k pages, black ($117/catridge)
2.3k Pages, coloured ($138/catridge, CMY)
2 black refills a year, 1 colour refill every 2 years
Don’t need to refill drum ($200, 50k pages refill if needed)
70W printing, 10W idle, 0.04W off
Relatively quiet
Up to A4 prints
250 sheet capacity
26PPM
<br/>
<br/>

HL-L3230CDN Laser Printer ($358) (Discontinued when rewriting the Readme file):

3k pages black ($121/catridge)
2,3k pages, coloured ($143/catridge, CMY)
2 black refills a year, 1 coloured every 2 years
1 refill of drum is needed for 5 years ($221, 18k pages)
75W printing, 8.8W idle, 0.04W off
250 sheet capacity
Up to A4 Prints
18PPM
<br/>
<br/>

Power cost (in order):

940h printing, 1410h idle/ready(HP), 6410h off
<br/>
<br/>

5170, 1269, 192.3 : $1991.38
391040, 1672, 320.5 : $118,027.66
68500, 14100, 256.4 : $24,881.78
70500, 12408, 256.4 : 24,974.27
<br/>
<br/>

Paper cost:

Total paper use = 34250 = 68.5 REAMS
Assuming company has a contract with PaperOne for 70g paper
100 REAMS at 3.45/REAM = $345
Used = ~$236.33
<br/>
<br/>

TCO (in order):
718 + 1000 + 236.33 + 1991.38 = $3,945.71
599 + 3921 + 118027.66 + 236.33 = $122,783.33
368 + 2412 + 24881.78 + 236.33 = $27,898.11
358 + 24974.27 + 2,497 + 236.33 = $28,065.6

*this is before adding maintenance/repairs, which can be up to around 10-20% of TCO, as well as accounting for inflation
<br/>
<br/>

Conclusion:
For Company “A”, the HL-L3240CDW Laser Printer is the best printer for them as it has the lowest TCO.
<br/>
<br/>

Reflection:

If the printer was for home user that prints 5 pages a day, the best printer (for TCO) changes. However, if I were to choose from the 4 options I gave, it would be the HL-L3230CDN Laser Printer, as it is cheaper to purchase as although it has a higher TCO for a company, it would be significantly lower for a home user as significantly lesser prints is done and the user can unplug the printer from the power outlet when not in use.
<br/>
<br/>

Apart from TCO, the printer’s capability, compatibility and upfront cost also needs to be taken into consideration when choosing. If the company was an arts company that prints artwork, than the MFC-J3940DW Inkjet Printer would have been the better choice as it is an InkJet printer.
<br/>
<br/>

For a large workgroup, the ideal printer would have a high PPM count, high sheet capacity and good reliability as we want to reduce the time wasted on waiting for a printer to finish it’s task, time used to refill the paper tray and resources spent/hours wasted on repairs
Assuming that the chosen printers don’t break down, the TCO gap between all of them will remain the same. However, the only time the TCO will the same is if one printer keeps breaking down and require maintenance/repairs.


##########################################################################
<br/>
<br/>

Session 2b - PM
<br/>
<br/>

##########################################################################

Cloud Computing:

*As I do not have a credit card, i cannot sign up for AWS, or similar services that require me to enter my credit card information in order to register.

I will start with configuring a firewall (on UFW)

when trying to ping without firewall

<img width="812" height="576" alt="pingoff" src="https://github.com/user-attachments/assets/2de85f41-9a4e-448a-858b-672901ffee7f" />
<br/>
<br/>

when trying to ping with firewall

<img width="814" height="577" alt="pingon" src="https://github.com/user-attachments/assets/333511c9-7cf7-4a38-8e86-68fb30bbfd1a" />
<br/>
<br/>

when trying to ping after giving permission to port 80

<img width="813" height="579" alt="pingperms" src="https://github.com/user-attachments/assets/5af9e8c3-3e97-4040-8b27-7c697f6391ec" />
<br/>
<br/>


SSH

*for this section of the lab, I will be executing the SSH from a cloned VM. I have created a new user "test" in the main VM and allowed connection to port 22 in the firewall
<br/>
<br/>

when logged in via ssh

<img width="813" height="579" alt="sshLogin" src="https://github.com/user-attachments/assets/2fc757b7-15c1-4e97-a5b6-bcafff0ddb3a" />

<br/>
<br/>

after updating

<img width="977" height="601" alt="sshUpdate" src="https://github.com/user-attachments/assets/3a6bffad-3acc-4394-a0ef-dda3bba810fd" />

<br/>
<br/>

BASH Scripting:

*all scripts will be saved inside ISEA file in documents

creating bash script

<img width="1204" height="581" alt="createbash" src="https://github.com/user-attachments/assets/08d3c6a6-416e-45cf-83b8-174a425ba3a7" />
<br/>
<br/>

converting file into executable

<img width="1202" height="571" alt="bashExec" src="https://github.com/user-attachments/assets/d1183e24-3855-46aa-a438-2ddba402bee9" />
<br/>
<br/>

echo message

<img width="816" height="582" alt="bashecho" src="https://github.com/user-attachments/assets/9719f4e3-d377-4e36-a92e-20d4319ce99b" />

*code
<br/>
<br/>

<img width="1203" height="409" alt="bashechoexec" src="https://github.com/user-attachments/assets/468a7173-54a1-4d14-b4c8-8ce5596efdc0" />

*output

if else

<img width="816" height="582" alt="bashif" src="https://github.com/user-attachments/assets/432a1004-9fff-4a63-8838-2bb5d35dab4a" />

*code
<br/>
<br/>

<img width="817" height="580" alt="bashifexec" src="https://github.com/user-attachments/assets/6a0a4f24-ffbb-4d59-9cfc-e1ea0377819b" />

*output
<br/>
<br/>

for loop

<img width="817" height="583" alt="bashfor" src="https://github.com/user-attachments/assets/932dc458-f5ae-4d63-8e45-220a40c5d1e7" />

*code
<br/>
<br/>

<img width="815" height="580" alt="bash4exec" src="https://github.com/user-attachments/assets/054b26c1-c514-4cc1-ba3b-f25c5b7286b8" />

*output
<br/>
<br/>

while loop

<img width="818" height="582" alt="bashwhile" src="https://github.com/user-attachments/assets/0f5551f9-b02b-4122-9d97-97752017b2d6" />

*code
<br/>
<br/>

<img width="820" height="582" alt="bashwhileExec" src="https://github.com/user-attachments/assets/769e411e-c84c-432e-91cb-b17111c59564" />

*output
<br/>
<br/>

for cron

crontab file: 

<img width="818" height="584" alt="crontab" src="https://github.com/user-attachments/assets/45e14af5-a65b-4a1f-833e-8def80b2624b" />

*in the 1st cron rule/setting, the script will run on the 17th min of every hour
<br/>
<br/>

when i want to run the script, i can use "bash" or 
"./". chmod simply only remove/add permissions to the file to user groups (default is editing permissions to all user groups)

output


<br/>
<br/>

##########################################################################
<br/>
<br/>

Session 3 - AM
<br/>
<br/>

##########################################################################

<br/>
As i do not have a credit card, there is nothing i can show for both labs in this session (both are reliant on AWS).
<br/>
<br/>

##########################################################################
<br/>
<br/>

Session 3 - PM
<br/>
<br/>

##########################################################################

Scripting Linux Server Functions:

*source directory for backups would be ISEA, and the target directory would be ISEA_BP

script

<img width="815" height="584" alt="backup" src="https://github.com/user-attachments/assets/be45425f-d486-4ece-9a68-96b3001de554" />

*file has been moved to a common folder for ease of access

<br/>
<br/>

before backup

<img width="938" height="637" alt="b4backup" src="https://github.com/user-attachments/assets/b99cbdc5-524a-444f-9736-fdc09a62cc86" />

<br/>
<br/>

after backup

<img width="1016" height="714" alt="afterbackup" src="https://github.com/user-attachments/assets/0e1964b8-919c-4cc9-90d6-b4cb82ca3798" />

<br/>
<br/>

using cron to schedule when does script run (i will run the backup script once every 2 mins)
<br/>
<br/>

code change (to produce an output)

<img width="971" height="600" alt="codechange" src="https://github.com/user-attachments/assets/db660b5d-506c-4ddd-a485-93d0251d942f" />

<br/>
<br/>

crontab

<img width="1057" height="601" alt="autorun" src="https://github.com/user-attachments/assets/99b70d85-3457-4697-b565-731606941a3a" />

<br/>
<br/>

log

<img width="704" height="521" alt="cronLog" src="https://github.com/user-attachments/assets/ab99df51-610e-479f-ad4a-57fdf518e28a" />


*log directory is in Documents

**log was updated whilst i was taking a screenshot

<br/>
<br/>

##########################################################################
<br/>
<br/>

Session 4a - AM
<br/>
<br/>

##########################################################################

Using MariaDB:

As I do not have an AWS account, remote access to the MariaDB server will be done via ssh.

The goals I have set is to create a user account (and a password for account), create/delete databases, create/delete tables and adding/deleting data to table on one VM (Virtual Machine), and seeing the changes in another VM


To install MariaDB:

<img width="816" height="578" alt="installMaria" src="https://github.com/user-attachments/assets/ab57188d-e8a5-49bc-9fbf-861ad9f24111" />

<br/>
<br/>

To setup MariaDB (and root account):

<img width="817" height="580" alt="setupMaria" src="https://github.com/user-attachments/assets/1b07d2df-b408-4563-bb90-f3410128a7f5" />

*root accoount password can be changed in this step.

<br/>
<br/>

To login to MariaDB:

<img width="815" height="578" alt="loginMaria" src="https://github.com/user-attachments/assets/f1999a5d-09e4-4b21-ac37-c5a54ecf86b0" />

*note that root account is needed for 1st time as no user account has been made (will login as root/admin)

** replace "root" with username if account has been made already

*** sudo can be used to bypass password requirement

<br/>
<br/>

To create a new user (username = test2, password = a):

<img width="818" height="586" alt="createUserMaria" src="https://github.com/user-attachments/assets/432f15e8-ac1c-4580-8199-09d7b75e9178" />

*you can replace "test2" with desired username, and "a" with desired password

<br/>
<br/>

To delete user (test2):

<img width="816" height="579" alt="userlistMaria" src="https://github.com/user-attachments/assets/7bcdc3a9-4c8e-42b3-89b0-fc3d0687ba26" />

*user list before deleting

<img width="818" height="583" alt="deleteUserMaria" src="https://github.com/user-attachments/assets/8add029e-e70b-4aac-9b15-f1797cd766e4" />

*user list after deleting

<br/>
<br/>


To create database:

before creating

<img width="814" height="579" alt="showdatabaseMaria" src="https://github.com/user-attachments/assets/ae86615f-9561-4437-8e19-07e7fa845f23" />

<br/>
<br/>

after creating

<img width="816" height="577" alt="createDatabaseMaria" src="https://github.com/user-attachments/assets/374bf367-9308-4528-919d-4148f75737e0" />

<br/>
<br/>

To delete dabase (deleting ISEA_Test2):

<img width="815" height="581" alt="deleteDatabaseMaria" src="https://github.com/user-attachments/assets/3e80e527-3889-44cd-9610-7758481e209a" />

*note that to delete database, permissions must be given to account, else only root account can delete them
<br/>
<br/>

To create table (in database):

Entering a database (similar to cd in linux console)

<img width="816" height="583" alt="enteringDtabaseMaria" src="https://github.com/user-attachments/assets/af85cd83-1aa7-49d7-8419-fb48583a0de4" />

*this step is not needed to create a table if you define which database you want to create the table in

<br/>
<br/>

create table (auto index 1st coloumn, text for 2nd coloumn)

<img width="815" height="584" alt="createTableMaria" src="https://github.com/user-attachments/assets/28558d7b-111b-4a6c-9f80-c441140a16ff" />

<br/>
<br/>

table view

<img width="817" height="581" alt="showTablesMaria" src="https://github.com/user-attachments/assets/505940b6-5ad8-4552-b07c-f532bbb80f5e" />

<br/>
<br/>

To delete table:

<img width="817" height="579" alt="deleteTableMaria" src="https://github.com/user-attachments/assets/149747b9-1570-4806-8748-db6e00c65893" />


<br/>
<br/>

To add data (adding a famous line from a sci-fi movie :D ):

<img width="817" height="577" alt="addingData" src="https://github.com/user-attachments/assets/45aa5114-f22a-4187-bc26-3bc895fa2b79" />

<img width="820" height="585" alt="delDataTestMaria" src="https://github.com/user-attachments/assets/27a785af-0a9b-444e-b107-8f0a779537fa" />

*data entry must match what data type is expected when creating the table

<br/>
<br/>

To delete data (removing data with id 2):

<img width="819" height="581" alt="deletedataMaria" src="https://github.com/user-attachments/assets/bab4f1cf-14b1-4c84-8693-a7e267564dc9" />

*note that drop command removes the data entry with specified data. unique data to be used unless you want to delete multiple data points

<br/>
<br/>

Granting Permissions:

*its important to mantain data security and integrity

<img width="814" height="579" alt="permissionsMaria" src="https://github.com/user-attachments/assets/69e22f2c-d18b-4d01-8cc1-ddd9fc4823a2" />

<br/>
<br/>

new perms (i have granted perms to mydatabase prior)

<img width="672" height="582" alt="pemrsMariadb" src="https://github.com/user-attachments/assets/17496bae-2c56-4f2a-a9bf-3cc7fccbbac7" />

*note that mariadb doesnt warn if you are granting permission to a database that never existed

** *.* can be used in place of database name if you want to give access to all databases in server

<br/>
<br/>

Removing Permissions (removing mydatabase):

<img width="954" height="580" alt="removepermsMaria" src="https://github.com/user-attachments/assets/d37db9f3-e683-4ce3-96db-83b4ef2cba6f" />

new perms 

<img width="954" height="581" alt="newpermsMaria" src="https://github.com/user-attachments/assets/623bf3d8-05cc-4069-a464-1ebdccc191dd" />

<br/>
<br/>

Remote Access (Adding data to ISEA_Test, from clone VM):

SSH View

<img width="1283" height="886" alt="clonedLoginMaria" src="https://github.com/user-attachments/assets/647a8aee-72c1-4a46-a393-98db19457080" />

*note the VM's name in the top left

**MariaDB can login remotely without using SSH if configured for it according to my research

***Remote user needs to install MariaDB-client-core before being able to remotely login if not done via ssh to VM hosting MariaDB

****Port configured for MariaDB must be open in firewall to connect to MariaDB without using ssh. Default port is 3306

<br/>
<br/>

after adding a few data entries

<img width="1282" height="886" alt="coupleoflinesMaria" src="https://github.com/user-attachments/assets/5665024e-b687-4e5d-a178-3d0074163e80" />

*this is the view of the table in the database

<br/>
<br/>

local view

<img width="1283" height="885" alt="localViewMaria" src="https://github.com/user-attachments/assets/e8c40ba2-0810-4f05-bd58-21369e189821" />

*again, note the VM's name in the top left

<br/>
<br/>

**End of Document**

