
So upfront you woud want to install vscode. Download it from this website: [downloadLink](https://code.visualstudio.com/)  
After successfully installing it you should see the window like this:  
![image](https://github.com/XinhaoZhao/cse15l-labReport1/blob/main/img1.png)  
  
  
  
Then, Install openSSH.  
After you install openSSH, try logging into the course specific account.  
A successful login should look like this:  
![image](https://github.com/XinhaoZhao/cse15l-labReport1/blob/main/img2.png)  
  
  
Next, try to run some commands using ssh. For example, try `$ ls -lat`.  
You should get something similar to this:  
![image](https://github.com/XinhaoZhao/cse15l-labReport1/blob/main/img3.png)  
  
Then, try moving files remotely using scp. Use the command `$ scp WhereAmI.java cs15lfa22zz@ieng6.ucsd.edu:~/ `.  
(Assume you already have a java file called WhereAmI.java)  
Again, log into ssh and use the command "ls" to see if the file is moved there.  
![image](https://github.com/XinhaoZhao/cse15l-labReport1/blob/main/img4.png)  
