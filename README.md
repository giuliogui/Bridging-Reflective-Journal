1. Introduction
This is my reflective journal, it will document my introduction to Server Environments and Architecture module learning experience. It will cover sections of the hand on experience Linux setup, command, scripting, network, security, automation and more. I used Ubuntu in both my Azure cloud environment and virtualization machine, downloading and configuration services such as Apache, securing my system with port 80 and 443 and wrote basic bash script. Even though Some of the labs are difficult such as scripting and writing bash, i still challenge myself to finish them or find alternative ways to finish them. This module has lay a sturdy foundation in experiencing as real IT role.

2. Linux Environment Setup

<img width="900" height="182" alt="image" src="https://github.com/user-attachments/assets/d9c7f9e6-2b1a-4198-bf95-2df9c93cd3e5" />

In this screenshot it shows that I successfully downloaded Ubuntu-24.04.3-desktop-amd64.iso
From the official ubuntu website. The ubuntu I downloaded file size is 3.5GB. 
What I learned:
I learned to identify the correct version of ISO for my setup and the importance of downloading and using the official sources to avoid any malware or disruption.

<img width="788" height="485" alt="image" src="https://github.com/user-attachments/assets/85a0fbc3-e609-4c2e-93cb-6c2310df3e04" />

In this screenshot it shows that I use Ubuntu Terminal to install VirtualBox Guest Additions by typing this command in “sudo apt install virtualbox-guest-utils”. This allows me to resize my screen and clipboard sharing between host and guest OS. This helps improve the Ubuntu environment’s usability and more importantly allows me to copy commands from labs.

<img width="868" height="460" alt="image" src="https://github.com/user-attachments/assets/3768d4e7-4c1d-4903-99ed-08fbb1e081f9" />

Oracle VirtualBox Manager interface. It shows that the Ubuntu is running and shows the configuration details I did on my Ubuntu. I named my VM “Ubuntu” for simplicity, the key setting I configure during installation is changing the Base memory to 4096 MB of RAM doubling the minimum recommended in the lab, 2 CPU cores and 10 GB virtual hard disk. I also set the network adapter to NAT mode, NAT allows me to isolate the VM from my local network while still having access to internet.
 
3. GitHub Integration and Usage

<img width="470" height="408" alt="image" src="https://github.com/user-attachments/assets/63e54f7f-333f-442d-8d44-1323bbcd5b53" />

My GitHub repository creation page where I set up new repository named Bridging Reflective Journal. I set the visibility public. I will use this GitHub repository to showcases what I learnt during this module.

4. Linux Services, Permissions, and Bash Scripting

<img width="735" height="450" alt="image" src="https://github.com/user-attachments/assets/f89a0346-0766-4d16-ae50-472bda39add8" />

output when using ps -e, it lists Ubuntu system running processes. This command is helpful because it can be used to identify any running services and see the amount of resource usage used by processes.

<img width="789" height="494" alt="image" src="https://github.com/user-attachments/assets/26301eb1-d78b-4587-a996-c83b395fdef6" />

 “top” command. it provides a view of system performance, CPU. Memory usage and more. This command can be used to monitor system load changes and resource usage while running applications. 
Ps -e provide a static snapshot of system activity while top provide a dynamic real time view of system performance.

<img width="741" height="170" alt="image" src="https://github.com/user-attachments/assets/1223e151-04c4-49ec-8e38-18273d0fa872" />

“ls”, this command displays files that can be found in the home folder.

<img width="787" height="383" alt="image" src="https://github.com/user-attachments/assets/61ee6ac2-91fa-4927-94a0-5462230b88bb" />

“ls -la”, this command allows the user to view all the hidden files and detailed permission in the system. Example: .bashrc

<img width="781" height="386" alt="image" src="https://github.com/user-attachments/assets/baffb3ac-9cda-4888-b9d8-e213cf1fa2d7" />

“ls -alt”, this command allow the user to view all files like ls -la command but the files are sort In modification time from newest to oldest.

<img width="900" height="463" alt="image" src="https://github.com/user-attachments/assets/5835d4ce-0e98-452d-9ff8-5cb629ed85ae" />

“ls -lah”, this command allows the user the view all files but it display the files size in human readable language.

<img width="710" height="436" alt="image" src="https://github.com/user-attachments/assets/65f876ac-5ae3-48f0-a7e0-a4b50e3ce1dc" />

 “touch”, this command is used to create files using terminal

 <img width="900" height="85" alt="image" src="https://github.com/user-attachments/assets/878820cf-0eab-4a2e-82c2-25bbbbdefa41" />
 
 “nano”, this command is used to edit the content inside the file

<img width="900" height="422" alt="image" src="https://github.com/user-attachments/assets/8a90758e-0fbf-4f06-876a-1b2ad2cacdc0" />

The result of using nano, it shows the terminal open the file and I was able to edit inside the file and I typed “This is for practice part 2” in the file.

<img width="841" height="109" alt="image" src="https://github.com/user-attachments/assets/51b21675-1dca-4399-bd5d-73f18f0ab2a5" />

This screenshot shows “cat”, this command allow me to see what I typed in the file using the terminal which was “This is for practice part 2”.
What I learned:
“gedit” and “nano” is both are used to edit files but “gedit” is more user friendly because it has a graphical interface while “nano” run in the terminal allowing u to edit the file content in the terminal. 

<img width="713" height="486" alt="image" src="https://github.com/user-attachments/assets/2956102b-4ccf-49b9-89d7-c8ab8dcace06" />

“cp”, this command allows to duplicate a file as shown in the screenshot.

<img width="774" height="528" alt="image" src="https://github.com/user-attachments/assets/e128e743-c074-43da-9dcb-2d76cd50af83" />

“mv”, this command allow user to rename the file named as shown In the screenshot from “proof_cp.txt” to “renamed_cp.txt.

<img width="774" height="498" alt="image" src="https://github.com/user-attachments/assets/dcdb2df3-083e-4ba1-8837-810bd9b42ef8" />

“rm” this command allows user to delete a file using the terminal.

<img width="900" height="130" alt="image" src="https://github.com/user-attachments/assets/faff91fe-89f4-403e-9a96-bade45ae2161" />

Uname -a command displays my ubuntu system information detailed such as kernal, host, and architecture details.

<img width="709" height="213" alt="image" src="https://github.com/user-attachments/assets/11ef2148-69ea-4831-99de-84730d888dd1" />

Lsb_release -a, it displays distribution details such as release, codename and description

<img width="803" height="525" alt="image" src="https://github.com/user-attachments/assets/1bbb8d96-b833-4d99-bdf3-e9f154d7ae44" />

hostnamectl, it displays the system hostname, virtualization details, architecture and other details.

<img width="520" height="75" alt="image" src="https://github.com/user-attachments/assets/8afa7f0a-7384-4864-8289-b63c9384fb60" />

“whoami”, it shows the current user

<img width="505" height="109" alt="image" src="https://github.com/user-attachments/assets/078ab03b-47af-47fc-80b4-fcc2820821d1" />

“sudo whoami”, “sudo” temporarily give u root privlleges for the next command and running “sudo whoami” it switches my identify from being a normal user to a root user.

•	`adduser` as sudoregular user, then with `sudo`.
<img width="900" height="78" alt="image" src="https://github.com/user-attachments/assets/4f6d7cb6-042d-432e-b515-c54e3e7d716e" />

“adduser”, this command run into error since only root can add a user into the system

<img width="879" height="405" alt="image" src="https://github.com/user-attachments/assets/ba47cb1b-59be-4c03-b108-d54dfadda571" />

“sudo adduser”, by using “sudo” I was allowed to add new user since im adding as a root.

<img width="900" height="329" alt="image" src="https://github.com/user-attachments/assets/8906cf05-74c3-4f39-968e-3b8b70182e9a" />
<img width="900" height="306" alt="image" src="https://github.com/user-attachments/assets/a16a3443-2451-4d94-bf00-82d346be1359" />

“ip a”, this shows networks details, including private IP. while public IP, it is shared by the entire home to access internet, 

<img width="900" height="319" alt="image" src="https://github.com/user-attachments/assets/8654034c-c6de-422e-9af0-7c74fb3008e6" />

“ping -c 4 8.8.8.8”, this test the network to google public DNS server. It shows an  latency and four packet transmitted with 0% packet loss. 
What I learned:
DNS stands for domain name system, the purpose of it is to translate user friendly names such as google.com into what computers can understand or known as IP addresses such as 142.222.72.222.

<img width="897" height="471" alt="image" src="https://github.com/user-attachments/assets/bcc05ae4-94c0-4564-8f30-2da4f69107b9" />

Sudo nano /etc/hosts, added a custom aliases, (GoogleEpicDNS > 127.0.01.)

<img width="739" height="539" alt="image" src="https://github.com/user-attachments/assets/34b08806-f746-47a5-8195-fa560760ee96" />

Ping -c 4 GoogleEpicDNS, i ping the custom aliases and it was successful.

<img width="369" height="482" alt="image" src="https://github.com/user-attachments/assets/d6c17b7d-931c-4ef5-9662-7bc5d65f7f8f" />
<img width="396" height="477" alt="image" src="https://github.com/user-attachments/assets/a1ab8b5b-d110-4136-bf3f-f984c2a61b5e" />

Nslookup, this command resolves domain names into IP address, (google.com>142.251.32.110) 
Sudo apt install whois, installed the whois client, this client is a tool that see domain registration and ownership.

<img width="663" height="406" alt="image" src="https://github.com/user-attachments/assets/d20849be-0718-4202-8a58-deee99edca78" />

whois google.com, it shows details of google.com domain owner, registration/expiry dates and more.

<img width="900" height="128" alt="image" src="https://github.com/user-attachments/assets/4a519224-c622-4bde-b84f-37008978ce38" />

lsusb, it lists all the USB devices 

<img width="900" height="218" alt="image" src="https://github.com/user-attachments/assets/1dffc472-7a6b-4b73-8c8d-e14cea205deb" />

Lspci, it list PCI bus and device connected to it.

<img width="900" height="552" alt="image" src="https://github.com/user-attachments/assets/9126ed11-c53e-4944-80cd-77d502d985e4" />

The result of less /proc/cpuinfo shows CPU information such as cores, model and flags.

<img width="527" height="249" alt="image" src="https://github.com/user-attachments/assets/cb12e50f-4b29-469c-9af2-8e3fcdf55276" />
<img width="498" height="318" alt="image" src="https://github.com/user-attachments/assets/124e4e57-2501-4a58-a2a3-0ed300203b54" />
<img width="503" height="306" alt="image" src="https://github.com/user-attachments/assets/070e6136-e24c-44f3-bfb7-759be242f783" />

Sudo apt update, upgrade and installed VLC using apt install.

<img width="504" height="470" alt="image" src="https://github.com/user-attachments/assets/711f5a31-6987-4145-b04b-d6d78617f2d4" />

Apt search, it explore all available packages, (VLC packages), it list the packages information.  Apt search is tools that help with discovering software without using the web.

<img width="900" height="550" alt="image" src="https://github.com/user-attachments/assets/7ee38d2e-69a6-48c2-b937-cb3dae008385" />

Installed Apache, using install command, tested the status, started it, test web “127.0.01” and install SSH server and Nmap. I learned Linux services run even if no one logged in.

<img width="900" height="562" alt="image" src="https://github.com/user-attachments/assets/cfde9a4b-1740-4b0f-82a4-83c3ab5d0711" />
<img width="900" height="410" alt="image" src="https://github.com/user-attachments/assets/26728501-daa5-476a-9245-8156312933c3" />

Different between apache removal, removing it made port 80 disappeared, the benefit of it is fewer entry point and harder to compromise and hackers can’t see and attack the web server.

<img width="850" height="81" alt="image" src="https://github.com/user-attachments/assets/7ed095bd-4a0c-4d7c-8392-a1b9b3c8b990" />
<img width="603" height="172" alt="image" src="https://github.com/user-attachments/assets/a012db1b-4a5a-4574-bd6d-e013623170c8" />
<img width="900" height="328" alt="image" src="https://github.com/user-attachments/assets/7b467489-afd8-46ed-bbe4-64ab40037d7c" />

Enabled UFW and allow port 80, it let only web traffic (HTTP) and blocks all unwanted traffic. Keep it secure and accessible.

<img width="459" height="371" alt="image" src="https://github.com/user-attachments/assets/fd04435a-635d-41ce-bdfa-c99f524b9f9d" />
<img width="419" height="371" alt="image" src="https://github.com/user-attachments/assets/9cd5896c-36eb-47ec-aa6c-7f3eb4fde5da" />

cloned my VM and made them shared NAT network, allowing both to communicate.

<img width="858" height="525" alt="image" src="https://github.com/user-attachments/assets/a6bdd701-3ab4-4adc-b360-cb7b96ccdc42" />

“Sudo adduser”, this make you a temporarily root and allow you to add new user.
Doing “adduser” without “sudo” will make the system reject it because only root can add new user.

<img width="669" height="375" alt="image" src="https://github.com/user-attachments/assets/7c0afc2a-7cee-4efa-b114-80cc7a5a4612" />

“sudo groupadd sharedgroup”, create new user group (sharedgroup), make it easier to manage permission for multiple user at once.
“sudo mkdir /home/shared”, create directory inside /home (shared). Allow multiple user files access.
“sudo touch /home/shared/file{1..10}”, create 10 empty files in the shared directory.
“sudo chgrp -R sharedgroup /home/shared”, change /home/shared group owner to sharedgroup. -R = recursive.
“sudo usermod -aG sharedgroup”, add a user as secondary group member to sharedgroup.
“sudo chmod -R 770 /home/shared”, sudo chmod 750 /home/shared/, it gives permission on shared directory and files inside. 
7 (owner): read + write + execute
5 (group): read + execute (no write)
0 (others): no permissions

<img width="472" height="244" alt="image" src="https://github.com/user-attachments/assets/f2b28e2b-bb7c-46cd-84df-4f82ebf21c35" />

“groups Mallory” shows what group is Mallory in.
“Sudo sudo gpasswd -d Mallory sharedgroup”, remove Mallory from sharedgroup.

<img width="673" height="228" alt="image" src="https://github.com/user-attachments/assets/cc8ec5d1-067b-49bb-8ba8-260c2a27ab34" />

“sudo usermod -aG sudo Mallory”, this add Mallory to sudo group
“su -mallory”, this switch to the user Mallory

<img width="900" height="101" alt="image" src="https://github.com/user-attachments/assets/8926b04f-9683-4047-b75b-20fd12b0f992" />

Ls -lh *bz2, it lists all files that end with *bz2 in human friendly readable way, this is important before running bunzip2 to prevent errors, save time and avoid using command on the wrong files.

<img width="900" height="143" alt="image" src="https://github.com/user-attachments/assets/4a1f7870-9270-4499-94ce-e970ff608d51" />

Bunzip2 and tar -xvf, Decompressed and extracted Gutenberg, this command is essential for managing software, backups and datasets.

<img width="900" height="174" alt="image" src="https://github.com/user-attachments/assets/0c291873-b238-4acb-9947-08067c19212b" />

find, searches 1b-3-Gutenberg directory, subdirectories to find files that contain .txt extension. This command is efficient for data cleanup and log analysis.

<img width="900" height="78" alt="image" src="https://github.com/user-attachments/assets/97301c4a-ba75-48b0-9472-9fb0785ada6e" />

Does recursive search through files directory, finding a keyword or phrase, display the line where it appears

<img width="900" height="94" alt="image" src="https://github.com/user-attachments/assets/f2a79c9e-1f10-4189-97f5-2d299eb24817" />

Does recursive searches  for phrases or keyword In a directory and display the 3 lines before and after  at the keyword or phrases.

<img width="900" height="111" alt="image" src="https://github.com/user-attachments/assets/ba1399b7-d83f-4658-b1d0-1cc15c840432" />

Searches for files in a directory with 52 bytes size and display their details like size, date and permission.

<img width="900" height="126" alt="image" src="https://github.com/user-attachments/assets/9d980d9f-8e3a-4432-9207-7c7289ff5501" />

Searches for in the directory, display their last known modification timestamp and path. (oldest to newest)

<img width="900" height="167" alt="image" src="https://github.com/user-attachments/assets/3fb7319c-813a-4a8f-a1bc-4b8a637b0775" />

Shows directory the biggest consumer files in a directory, useful for finding the files that taking all the disk space.

<img width="900" height="485" alt="image" src="https://github.com/user-attachments/assets/90bd0e73-6b48-44d1-be37-852e630f96de" />

Shows the most frequent word used in descending order.

5. Total Cost of Ownership (TCO) Azure vs AWS

<img width="942" height="347" alt="image" src="https://github.com/user-attachments/assets/07abd164-1d62-4185-a5c2-12a2853f328b" />
<img width="464" height="496" alt="image" src="https://github.com/user-attachments/assets/025b06ff-e693-445c-b2d3-900a84f279ee" />

I would recommend the student to choose Azure even though AWS is cheaper, because azure does not need to link a card to use it and it will not charge your card after credit is used up.

6. Provisioning and Securing a Cloud VM
<img width="900" height="448" alt="image" src="https://github.com/user-attachments/assets/63e115f3-dc75-4404-9119-4cc878c47d94" />
<img width="975" height="320" alt="image" src="https://github.com/user-attachments/assets/5899fe6e-f420-421f-bf26-8e7eea880c42" />

Created and launched Ubuntu 24.04.3 LTS

<img width="975" height="267" alt="image" src="https://github.com/user-attachments/assets/3e758aaa-1019-4342-868d-ea2e28e0371f" />

Security Group Configuration:
•	Opened port 22 (SSH) for secure remote administration.
•	Opened port 80 (HTTP) for web traffic.
•	Opened 443 (HTTPS) for redirect http traffic to https.

<img width="652" height="319" alt="image" src="https://github.com/user-attachments/assets/84d83f04-3228-4b69-8154-9bacaa21a952" />
<img width="667" height="353" alt="image" src="https://github.com/user-attachments/assets/816ddf19-8408-4eb2-8360-842b9347f15d" />

Connected to terminal, updated packages, installed Apache.

<img width="900" height="494" alt="image" src="https://github.com/user-attachments/assets/845e99e6-0d3e-43d7-99df-7920fa03fc4f" />
Used the public server IP to access server via web.

<img width="900" height="249" alt="image" src="https://github.com/user-attachments/assets/ad377e6a-0816-4882-93ee-3f1d34f5f372" />
<img width="900" height="228" alt="image" src="https://github.com/user-attachments/assets/6f6c5ab0-e3d0-425b-bc67-a8d87b04bf5d" />

Sudo nano, changed the web to my liking and test the live changes.

<img width="900" height="293" alt="image" src="https://github.com/user-attachments/assets/8996ac1c-1ba6-4481-bed7-8fd8870d09f3" />

Wget, it downloads files
Sudo cp, it copies files

<img width="900" height="203" alt="image" src="https://github.com/user-attachments/assets/18b4f400-891f-4302-9c71-d1c010dc110c" />
<img width="900" height="102" alt="image" src="https://github.com/user-attachments/assets/08a70ebc-0f3c-422a-90bd-b582d09fa344" />

<a> = create a clickable link
Href= “example” = link a file to the same directory
This command allowed a user to click on the “Download Sample PDF” to download a file.

<img width="705" height="392" alt="image" src="https://github.com/user-attachments/assets/0b488e3d-2e53-4920-8db3-1235e9175f1f" />
<img width="655" height="295" alt="image" src="https://github.com/user-attachments/assets/da74c349-ad0e-426c-9ede-949d57b7a29a" />
<img width="900" height="127" alt="image" src="https://github.com/user-attachments/assets/f9a4e9f9-682d-41f1-9c4f-1edbad7274d9" />

I set up a budget alert (budget subscription, monthly spending limit, added email notification if the spending reach 80% of the budget set via azure cost management, this help prevent overspending, teaches good habit to stop VMs when I’m not using. 

7. DNS Setup and SSL Configuration

<img width="900" height="478" alt="image" src="https://github.com/user-attachments/assets/9ee37173-8942-416d-904e-554b614a9234" />

I registered and created a domain using DuckDNS, it is a dynamic DNS service and allow a user to link an IP to a custom domain name. This allowed me to I linked my azure cloud VM public IP with a custom domain name. I also checked if my domain name is working by connecting to giuliogui.duckdns.org.

<img width="900" height="599" alt="image" src="https://github.com/user-attachments/assets/e6053a3e-63e5-428c-9e2b-4437f0c464f0" />

I checked my domain using whatsmydns.net. the result is dynamic, sometime an area has connection and other time it does not. 

<img width="900" height="320" alt="image" src="https://github.com/user-attachments/assets/502d12f4-c859-4f45-96fd-d27c452cbb4d" />

I also used nslookup to verify my DNS status.

<img width="900" height="449" alt="image" src="https://github.com/user-attachments/assets/bd2dc149-1e9a-4896-badf-ca8d2e899ce8" />

Installed Certbot and Apache plugin, this helped me add a layer of security to my domain (HTTPS).

<img width="900" height="595" alt="image" src="https://github.com/user-attachments/assets/02ac6152-ec1c-4b4d-94b9-ebd85a0bfc1b" />

This command allowed the system to create and install certificate for my DNS.

<img width="819" height="405" alt="image" src="https://github.com/user-attachments/assets/73d9362d-1549-4694-bfb8-1891f8c40f50" />
<img width="514" height="585" alt="image" src="https://github.com/user-attachments/assets/2fb076fb-bc69-403d-a103-470a245f324b" />
<img width="900" height="368" alt="image" src="https://github.com/user-attachments/assets/ccb8bc21-a6fc-4891-9caa-400cd77f5f6f" />

These screenshots prove my domain has HTTPS padlock and some certificate details.
After having SSL certificate from Let’s Encrypt, it will redirect any HTTP traffic to HTTPS.
Without HTTPS any data such as password, credit card information and sensitive data are sent in plain text between traffic of user and server. But with HTTPS, intercepted data are useless as they are encrypted (not readable).

<img width="900" height="332" alt="image" src="https://github.com/user-attachments/assets/c861478f-1d77-4b3d-bf85-a264e82f84b5" />

Dry run, a simulation renewal that does not actually renew. It checks if a certificate can be renewed when scheduled. It is important to dry run because it tests out if an error occur and avoid site issue when the certificate expires.

<img width="900" height="268" alt="image" src="https://github.com/user-attachments/assets/03f36f62-ebcb-4b04-b665-ab8fd879366d" />

I also explored alternative way to install cerbot by using snap.

<img width="900" height="209" alt="image" src="https://github.com/user-attachments/assets/a8b7f884-95cc-4996-8f4a-c2fde1d07343" />

This command allows me to ask the server what happen if someone connect using http (unsafe) instead of https, it replied with I will automatically send the user to https.

8. Automation and Cron Jobs
Writing Bash Scripts and Using Regular Expressions

<img width="743" height="464" alt="image" src="https://github.com/user-attachments/assets/9ad22c50-5063-426e-83b9-25a97a64eae4" />

Mkdir, it makes directory or in simple word create a new folder
Cd, it goes into the directory
Touch, it creates a file that empty
Cd, it creates a backup copy of the file
Mv, it renames file 
Rm, it delete the file

<img width="900" height="557" alt="image" src="https://github.com/user-attachments/assets/c6acc417-9d5c-42aa-8a9a-f0b964e551fc" />

Chmod 777, I made the file hello_world.sh executable for everyone without it, the file would only be just a text file.
./hello_world, this command allows me to execute the file and see the output of the file.

Learning Loops, Conditionals, and Debugging Bash Scripts

<img width="900" height="785" alt="image" src="https://github.com/user-attachments/assets/2f695fe0-8c36-4e3b-a804-146578e9d5de" />
<img width="900" height="347" alt="image" src="https://github.com/user-attachments/assets/0a44d794-f3e5-447a-9227-8b34b5f7fbf5" />

These screenshots are initial attempt to write bash and fail and use the bash script from SharePoint. I still ran into some error and couldn’t figure it out. IT successfully display the username and counting loop but the conditional statement ran into some syntax error. The second screenshot shows the successful output of first half then ran into errors. Though the script still works at the end showing “number out of range” but it was the wrong output, it should be “You entered a number less than or equal to 5.

<img width="900" height="102" alt="image" src="https://github.com/user-attachments/assets/2fd92a0a-b5c7-41c9-b6c7-c41f04875ef6" />

The command I used to edit the content inside resource-monitor (nano) and change file permission (chmod).

<img width="579" height="388" alt="image" src="https://github.com/user-attachments/assets/24104093-c13b-4c0e-b825-be0923e8b04c" />

This screenshot shows a working system monitoring script (resource_monitor.sh). The script works by asking the user how many time the user would like to monitor the system, then repeatedly run a loop to gather and display system metrics. There also a command called sleep that allow a user to observe the system changes easier.

<img width="716" height="481" alt="image" src="https://github.com/user-attachments/assets/1d30d8c0-1044-4ab5-a544-fdc74b90a81e" />

This is the output executing the “resource_monitor.sh”, it displays data such as CPU usage percentages, memory allocation, disk space usage on the main partition. 

<img width="716" height="441" alt="image" src="https://github.com/user-attachments/assets/74723d1a-9b75-4bfe-bcf4-d39ddc4e2886" />

Top, it display real time system statistic. It list program that are using my computer resources, similarly Window Task Manager.

<img width="900" height="86" alt="image" src="https://github.com/user-attachments/assets/b204f5a2-10a6-4b2d-ad36-c81441e581dd" />

Free-h, display the memory allocation in human readable languages.

<img width="900" height="256" alt="image" src="https://github.com/user-attachments/assets/7e5b4b85-d747-483b-b50a-4b1b988ffd01" />

Df -h, it displays disk utilization.

Scripting Linux Server Functions for Automation

<img width="900" height="357" alt="image" src="https://github.com/user-attachments/assets/6c8f47c3-bc4e-4e3b-8a41-955674131f1c" />

This screenshot shows I was using some command that required sudo because i was creating file as the user “Giulio” instead of “Ubuntu”. Using sudo allowed me gain temporary privileges to access the directory.

This is a backup script, it automates copying and zipping files based on current date.








