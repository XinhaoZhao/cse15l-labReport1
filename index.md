# **1. Installing vscode**  
So upfront you woud want to install vscode. Download it from this website: [downloadLink](https://code.visualstudio.com/)  
After successfully installing it you should see the window like this:  
![image](https://github.com/XinhaoZhao/cse15l-labReport1/blob/main/img1.png?raw=true)  
  
  
# **2. Installing openSSH and remotely connecting**  
Then, Install openSSH. Follow this link: [install open ssh](https://github.com/PowerShell/Win32-OpenSSH)  
After you install openSSH, try logging into the course specific account.  
A successful login should look like this:  
![image](https://github.com/XinhaoZhao/cse15l-labReport1/blob/main/img2.1.png?raw=true)  
![image](https://github.com/XinhaoZhao/cse15l-labReport1/blob/main/img2.5.png?raw=true)  
  
# **3. Trying some ssh commands**  
Next, try to run some commands using ssh. For example, try:  
`$ ls`  
`$ ls -lat`  
`$ ls -a`  
`$ cat /home/linux/ieng6/cs15lfa22/public/hello.txt`  
You should get something similar to this:  
![image](https://github.com/XinhaoZhao/cse15l-labReport1/blob/main/img3.1.png?raw=true)  
  
# **4. Try moving files using ssh**  
Then, try moving files remotely using scp. Use the command `$ scp WhereAmI.java cs15lfa22zz@ieng6.ucsd.edu:~/ `.  
(Assume you already have a java file called WhereAmI.java)  
Again, log into ssh and use the command "ls" to see if the file is moved there.  
![image](https://github.com/XinhaoZhao/cse15l-labReport1/blob/main/img4.png?raw=true)  
 
# **5. Generate ssh keys**  
Next to make logins more convenient you want to set a ssh key. Follow the commands in the following image to do that.  
![image](https://github.com/XinhaoZhao/cse15l-labReport1/blob/main/img5.png?raw=true)  
After this, follow this link [link](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_keymanagement#user-key-generation)  for ssh-add for windows users.  
Finally, use `$ scp <your file path> cs15lfa22@ieng6.ucsd.edu:~/.ssh/authorized_keys`  to move the public key to the .ssh directory created by using  
`$  mkdir .ssh`   
Now you should be able to login to ssh without actually entering your password

# **6. optimize ssh**  
Finally, to optimize ssh usage, you can type multiple commands in a single line. They will be executed in order.    
![image](https://github.com/XinhaoZhao/cse15l-labReport1/blob/main/img6.png?raw=true)  
