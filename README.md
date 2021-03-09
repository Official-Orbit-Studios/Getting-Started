# Getting Started here at Orbit

![Orbit Studios Logo](https://cdn.discordapp.com/icons/725472423511719938/a0635bd59280dac4ce4dd4e64aebd379.webp?size=128)

## Welcome to Orbit Studios!

Hey, welcome to our organization!

This tutorial will bring you up to speed on our workflow. 
The only thing this tutorial assumes is that your system is fully up-to-date

## Joining the organization

The first thing you will need to do is join the organization on GitHub. 
To do that we need your GitHub username so we can invite you. 
If we already have your GitHub username, chances are we've sent you an invite, which you can redeem from your email or at [our organization' profile page](https://github.com/Official-Orbit-Studios/)

## Setting up Git

Once you've joined the organization, it's now time to set up git!
Git is how we control our code. 
Linux users, you may find it in the package manager or preinstalled depending on your distribution. 
MacOS  users, you should have a copy of git on your system, although if you want a more up-to-date version, you can use [this tutorial](https://www.makeuseof.com/how-to-install-git-mac/). 
Windows users can download the executable installer from [their webpage](https://git-scm.com/). 
Leave all parameters to default. 
Once installed, git should be usable through the command line or terminal.
Set up your username by running `git config --global user.name "Your Name"` and set up your password by running `git config --global user.email "youremail@yourdomain.com"`
That's it, you're finished setting up Git

## Setting up SSH Keys for Git and GitHub (Recommended, but optional)

Now that you've set up Git, it's time to set up your SSH keys. These keys will make using Git a whole lot easier. 
First, start by generating an SSH key. 
These keys are specific to the machine your run them on, and you only need one per machine. 
On Linux and MacOS run `cd .ssh` to enter the .ssh directory. 
Then, run `ssh-keygen -t rsa` and hit enter to skip entering a passphrase.
On Windows, open the PowerShell as admin, and run `Add-WindowsCapability -Online -Name OpenSSH.Client~~~~0.0.1.0`
Then, run `ssh-keygen`, and hit enter to skip entering a passphrase.
then, do `cd .ssh`
This will generate a file called "id_rsa.pub"
You can view the contents of this file by running `cat id_rsa.pub` on Linux or MacOS, or by running `type id_rsa.pub` on Windows.
Copy the contents of the file, which should start with "ssh-rsa"
Then, go to settings in GitHub, and go to "SSH and GPG keys".
Create a new SSH key, and title it the name of your computer.
Then, paste the key you created earlier into where it says key.
Finally, save the key.

## Short Git tutorial (Skip if you know)

Note: This section requires you to have joined the organization.

We've now set up Git.
Now, we can clone repositories and help contribute.
To show you how, we've initialized a repository which you can clone and commit to.
Start by entering the folder where you keep all your projects.
Then, if you have [set up SSH keys](https://github.com/Official-Orbit-Studios/Getting-Started/blob/main/README.md#setting-up-ssh-keys-for-git-and-github-recommended-but-optional), run `git clone git@github.com:Official-Orbit-Studios/TestRepo.git`.
If you haven't set up SSH keys, run `git clone https://github.com/Official-Orbit-Studios/TestRepo.git`.
Run `cd` to enter into the new folder, and using your favorite editor, add your Discord username to the list of employees.
Once you've done that, add your changes to the local Git repository by running `git add -A`
Then, run `git commit -m "Message"`, with your commit message where it says message.
Once you've updated the list, you can push it back to GitHub by running `git push origin main`.
In case you need to update the repository with all the latest changes, you can run `git pull origin main`, to download all the latest changes for when you work on it.

That's it, you've learnt the basics of our Git/GitHub-based workflow!
Now, here's a short run down of what to do each day.

## Run Down

### First time

1. Run `git clone (ssh key or https url here)` to clone the repository locally
2. Edit the code
3. Run `git add -A` to add all your changes to be committed
4. Run `git commit -m "Message goes here"` to commit your changes locally
5. Run `git push origin main` to push all your changes to GitHub

And that's all there is to it! The workflow for once you've gotten started is pretty similar to that.

### Daily

1. Run `git pull origin main` to bring your local repository up to date with the one on GitHub
2. Edit the code
3. Run `git add -A` to add your changes to be committed
4. Run `git commit -m "Message goes here"` to commit your changes locally
5. Run `git push origin main` to push all your commits to GitHub

## Checklist

- [] Download and install (VSCode)[https://code.visualstudio.com] along with the [Live Share Extension](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare)
- [] Join the organization on GitHub
- [] Download and set up Git