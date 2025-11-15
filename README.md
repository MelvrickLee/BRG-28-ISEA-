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

checking service status using systemctl status
<img width="810" height="575" alt="systemctl" src="https://github.com/user-attachments/assets/0738aafa-496a-4322-8fb1-00c1f1d3fdb5" />

*only the 1st page as it is too long to document it all
<br/> 
<br/> 


Linux Permissions:

output for ls -l 

<img width="808" height="574" alt="permissions" src="https://github.com/user-attachments/assets/a614eb84-7ec7-482e-8ba6-9bd9ff2de027" />

*r means read, w means write and x means execute. the 1st column is for onwer, 2nd for group and 3rd for others. d denotes that the file is a directory
<br/>
<br/>

changing permissions (changing testfile to rw -r -r)




Session 2 - AM



Session 2 - PM



Session 3 - AM



as i do not have a credit card, there is nothing i can show for lab 1 and 2 (both are reliant on AWS).



Session 3 - PM

