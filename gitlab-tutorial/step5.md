# Create a File
In the project create a file `echo 'Hello, world.' > foo.txt`{{execute}}

# Add, Commit and Push Changes
First the user must be registered by typing `git config --global user.email "you@example.com"`. 
Prepare then all the files before the commit using `git add --all`{{execute}}. Next stage is to commit
the changes by doing the `git commit -m "test CI/CD server"`{{execute}}. Lastly, just push
the changes with `git push`{{execute}} command, where you may be asked to log in by typing 
your username and password. 

# Caveat!
Observe that the version of Git may be outdated on Katacoda. If everything works then this section may be ignored.
In the case that this causes problems, try using following commands to fix the issue: 


1. Remove the old version of git with: `sudo yum remove git`.

2. Download the new version of git: `sudo yum install -y https://repo.ius.io/ius-release-el7.rpm`.

3. Install the new downloaded version `sudo yum install git222`.

4. Run `git --version` to control that the right version is installed (git version 2.22.2).

5. Repeat step 5 in this scenario.