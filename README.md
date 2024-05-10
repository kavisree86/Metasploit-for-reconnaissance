# Metasploit-for-reconnaissance
# Metasploit
Metasploit for reconnaissance in pentesting

# AIM:

To get introduced to Metasploit Framework and to  perform reconnaissance  in pentesting .

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands
## Program:
Find out the ip address of the attackers system

## Output:
![image](https://github.com/kavisree86/Metasploit-for-reconnaissance/assets/145759687/7772eddb-ad19-4028-a290-bb17543c1470)

## Invoke msfconsole:
## Output:
Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.

![image](https://github.com/kavisree86/Metasploit-for-reconnaissance/assets/145759687/3dcd0766-62bf-47c4-9341-a3e040713806)





## Port Scanning Output: 
Following command is executed for scanning the systems on our local area network with a TCP scan (-sT) looking for open ports between 1 and 1000 (-p1-1000). msf > nmap -sT 192.168.1810/24 -p1-1000

![image](https://github.com/kavisree86/Metasploit-for-reconnaissance/assets/145759687/f3848008-bab1-4a4e-9ff0-a5bf54b4d5e3)



## Output:
![image](https://github.com/kavisree86/Metasploit-for-reconnaissance/assets/145759687/13597a21-159b-4816-ac23-374a11325f28)
the db-nmap command to scan and save the results into Metasploit's postgresql attached database. In that way, you can use those results in the exploitation stage later.

scan the targets with the command db_nmap as follows. msf > db_nmap 192.168.181.0/24


## output
![image](https://github.com/kavisree86/Metasploit-for-reconnaissance/assets/145759687/38deb71e-11fc-42e6-8ffa-0d49f79e2ff0)

Metasploit has a multitude of scanning modules built in. If we open another terminal, we can navigate to Metasploit's auxiliary modules and list all the scanner modules. cd /usr/share /metasploit-framework/modules/auxiliary kali > ls -l

## output
![image](https://github.com/kavisree86/Metasploit-for-reconnaissance/assets/145759687/70e56988-ee04-45a9-8295-709eb93275e7)
Search is a powerful command in Metasploit that you can use to find what you want to locate. msf >search name:Microsoft type:exploit

The info command provides information regarding a module or platform
## output:
![image](https://github.com/kavisree86/Metasploit-for-reconnaissance/assets/145759687/141c2fde-7619-4e98-8f1a-1726de5102cb)
Before beginning, set up the Metasploit database by starting the PostgreSQL server and initialize msfconsole database as follows: systemctl start postgresql msfdb init

## MYSQL ENUMERATION:
Find the IP address of the Metasploitable machine first. Then, use the db_nmap command in msfconsole with Nmap flags to scan the MySQL database at 3306 port. db_nmap -sV -sC -p 3306 <metasploitable_ip_address>
## Output
![image](https://github.com/kavisree86/Metasploit-for-reconnaissance/assets/145759687/9d4a9a18-4795-4ffd-b0c9-ca961e6562d9)

## output:
![image](https://github.com/kavisree86/Metasploit-for-reconnaissance/assets/145759687/62a3f8a8-e7ab-402a-9a7e-4efa6143ab6e)
set the PASS_FILE parameter to the wordlist path available inside /usr/share/wordlists: set PASS_FILE /usr/share/wordlistss/rockyou.txt Then, specify the IP address of the target machine with the RHOSTS command. set RHOSTS Set BLANK_PASSWORDS to true in case there is no password set for the root account. set BLANK_PASSWORDS true

![image](https://github.com/kavisree86/Metasploit-for-reconnaissance/assets/145759687/ff46bc6d-d24e-400f-a208-be9a12909e2b)










## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
