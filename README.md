# DevOps-HW0-Pipelines

> **My name is Khantil Choksi and unity ID is khchoksi.**  

## Completed Moodle and Slack profiles:
* **Moodle Profile:** ![img](/MoodleProfile.png)  

* **Slack Profile:** ![img](/SlackProfile.png)

## Computing Environment:
  * Using Baker:  
  
    
  * Using Vagrant

## Hook Script:
`#!/bin/bash`  
`open https://android.com`

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


