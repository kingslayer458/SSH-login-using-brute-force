# SSH-login-using-brute-force

SSH brute force tools are used to attempt to gain unauthorized access to an SSH server by
repeatedly trying different username and password combinations. These tools can be used
to attack both weak and strong passwords, but they are most effective against weak
passwords. Brute force tools are often used by attackers to gain access to servers and
other devices to steal data, install malware, or launch other attacks. However, SSH brute
force tools can also be used by security professionals to test the security of their own
systems and to identify potential vulnerabilities. This SSH brute force tool designed by us
will work by trying different username and password combinations by using the wordlist.
The wordlist is a text file which contains names or string characters which are used as
usernames and passwords. If the username and password are matched then, we can login
to the system or server using those credentials. The tool was designed by us using python
programming language. The tool requires username wordlist and password wordlist, port,
and host IP address

# how to set up ssh server in windows
Step 1: Check under “Settings” > “Apps” > “Optional Features” whether the SSH client is already installed. If the SSH client tool is not in the feature list, click Add Feature. Now search for “OpenSS Client” and select “Install”.The Optional Features menu with the Windows 11 OpenSSH client .By default, the pre-installed Windows 11 SSH client can be found under Optional Features.
Step 2: After installation, start the command prompt as administrator. This works in several ways, for example, by typing “cmd.exe” in the Windows search and then selecting the “Run as administrator” option.

#how to set up ssh server in linux
1. Open the terminal application.
2. Install the ssh package on Ubuntu by typing: **sudo apt install openssh-client**
3. Once the installation done, use it by typing from the CLIENT: **ssh user@serverip-here**


Now you know how to install ssh client. To accept connection for ssh session, you need to
install openssh-server package on Ubuntu. Hence, type the following commands.
1. Open your terminal application
2. Install the openssh-server package on Ubuntu, run: **sudo apt install opensshserver**
3. Enable ssh server on Ubuntu, run: s**udo systemctl enable ssh**
4. By default, firewall will block ssh access. Therefore, you must enable ufw and
open ssh port
5. Open ssh tcp port 22 using ufw firewall, run: **sudo ufw allow ssh**
6. Congratulations. Now you have SSH server installed and running on your
Ubuntu server. You can connect to it using ssh client.

   
# Command
open cmd type this command
python ssh-bf.py --users (dir of your user txt file) --passes (dir of password txt file) --host targeted ip address

for eg
python ssh-bf.py --users D:\PT1\pass.txt --passes D:\PT1\pass.txt --host 192.168.1.3
