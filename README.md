# Git and Git-hub set up GUIDE with Git Bash:

### STEP 1 - CREATE A GIT-HUB ACCOUNT

First thing to do, you need to create a github account if you have not done. In your account you will save all the repositories that you will be working.

### STEP 2 - INSTALL GIT BASH

Second thing to do, you need to install git from this [link](https://git-scm.com/downloads). Make you sure that you install the correct version for your device.

### STEP 3 - LOCATE THE WORKING FOLDER ON YOUR LOCAL MACHINE AND GENERATE SSH KEY

1. Open Git Bash
2. Go to your working folder where you would like to save your project in the local machine and create the new folder:
```
mkdir name_of_the_project
cd name_of_the_project
```
3. Type the following command to generate the SSH key:
```
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```
Press ENTER in all the steps, leaving empty the gap.

### STEP 4 - FIND YOUR KEY AND ADD THE KEY IN YOUR ACCOUNT OF GIT-HUB

1. Open GIT BASH
2. You should navigate to find the SSH key pair by using:
```
cd /c/Users/your_account/.ssh
```
List the directory by using:
```
ls -la
```
3. We could see our SHH key, that it corresponds with the .pub file, so let go to open the file by using:
```
cat filename.pub
```
4. You should see a long line of text in the terminal. Copy the whole text starting with "ssh-rsa".
5. Go to your account of Git-Hub and log in.
6. Click on your profile picture at the top of the right on the screen and after that click on the option of settings.
7. Find the option "SSH and GPG Keys" in the menu on the left of the screen and click on it.
8. Click on the option Add a new SSH key.
9. Write down a appropiate name of the Key related to the project, and paste the key in the key section.
10. Finally click add SSH key and we will save the public key in our account of Git-Hub

### STEP 5 - CREATE REPOSITORY ON THE COMMAND LINE

1. Open GIT BASH
2. Go back again in your folder where you will saved your project in the local machine.
3. Follow the following commands:
Create the file README
```
echo "# name_of_your_project" >> README.md
```
We initialize the repository
```
git init
```
Add the file README to the repository
```
git add README.md
```
Commit the changes with a brief description
```
git commit -m "first commit"
```
Change the branch
```
git branch -M main
```
Locate repository
```
git remote add origin https://github.com/your_name_account/name_of_repository.git
```
Push
```
git push -u origin main
```
4. Finally, go to your account of Git-Hub. Locate on the repository and you should all the changes that have done right now. You will be able to read your file README.md
5. YOU ARE DONE!
