# DevOps-HW0-Pipelines

> **My name is Khantil Choksi and unity ID is khchoksi.**  

## Completed Moodle and Slack profiles:
* **Moodle Profile:** ![img](/MoodleProfile.png)  

* **Slack Profile:** ![img](/SlackProfile.png)

## Computing Environment:
  * **Using Baker:**    
   * Here is my [baker.yml file](/ComputingEnvironment/baker.yml).     
   * Here is the [screencast](https://youtu.be/g_Pa-OYKTzw) demonstrating the creation of Virtual Machine, installing the NodeJS in it and synced folder.  
   * The following steps are to be done in order to perform the above task:  
      1. Install the Baker using homebrew.
       `brew install ottomatica/ottomatica/baker` 
      2. Setup the baker sever, to manage the Baker environments in machine.  
       `baker setup`  
      3. Create a simple Baker file that creates a VM at a given IP address and also install nodejs in your VM.  
  
       ```
            #baker.yml
            ---
            name: baker-computing   
             vm:  
              ip: 192.168.22.19  
             lang:   
               - nodejs9  
       ```      
       4. To Bake the virtual machine called `baker-computing`, the bake2 command is used with the `baker.yml` file path.   
        `baker bake2 --local`   
       5. After Baker finishes creating the VM, ssh to VM using `ssh` command.    
        `baker ssh baker-computing`  
       6. The directory where `baker.yml` is placed in local machine, becomes the synced folder in the VM.   
      
      
* **Using Vagrant:**  
  * Here is my [Vagrantfile](/ComputingEnvironment/Vagrantfile).     
  * Here is the [screencast]() demonstrating the creation of Virtual Machine, installing the NodeJS in it and synced folder.  
  * The following steps are to be done in order to perform the above task:  
      1. Install the Baker using homebrew.
       `brew install ottomatica/ottomatica/baker` 
      2. Setup the baker sever, to manage the Baker environments in machine.  
       `baker setup`  
      3. Create a simple Baker file that creates a VM at a given IP address and also install nodejs in your VM.

## Hook Script:
```
#!/bin/bash
open https://android.com
```

*I have done the following steps to implement the hookscript.*

* 1. git init .            // This will create a local repository in the present working directory.
* 2. nano ./.git/hooks/post-commit    //This will create a post-commit file in the hooks.
* 3. #!/bin/bash   //It’s written so that Unix/Linux shell knows what kind of interpreter to run the following commands, here it is Bourne Again Shell.  Then command open https://android.com
* 4. chmod u+x post-commit   //chmod is used to change the permission of the files like read, write and executable
* 5. Myfile.txt //To add something in the local repo so that we can commit and test our post-commit hook.
* 6. git add Myfile.txt //Add the file to local repo
* 7. git commit -m “New File” //Committing the changes to repo
* 8. This will open the link given in the post-commit executable file due to post-commit hook.


** Screencast:**




**Thank you for taking your valuable time and I hope that I had put my all efforts to understand the concepts of HW0.**


