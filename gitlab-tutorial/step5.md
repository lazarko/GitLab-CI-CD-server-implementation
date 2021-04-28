# Create a File
In the project create a file `echo 'Hello, world.' > foo.txt`{{execute}}

# Add, Commit and Push Changes
Prepare all the files before the commit using `git add --all`{{execute}}. 

Next stage is to commit the changes by doing the `git commit -m "test CI/CD server"`{{execute}}.

Git might ask you to register as a user. If so, enter `git config --global user.email "you@example.com"`, with your email and try to commit again.

Lastly, just push the changes with `git push`{{execute}} command. 

# Check the status of your pipeline

In your project go to CI/CD. You should see your pipeline at the top of the page and by clicking on the pipeline id you can see a visual representation of the pipeline. 

If everything works and all stages pass, congrats you have a working CI/CD pipeline and you can now alter the `.gitlab-ci.yml` file to fit your project.

If any of the stages fail, look at the next section.

# Caveat!
Observe that the version of Git may be outdated on Katacoda.
In the case that this causes problems, try using following commands to fix the issue: 


1. Remove the old version of git with: `sudo yum remove git`.

2. Download the new version of git: `sudo yum install -y https://repo.ius.io/ius-release-el7.rpm`.

3. Install the new downloaded version `sudo yum install git222`.

4. Run `git --version` to control that the right version is installed (git version 2.22.2).

5. Repeat step 5 in this scenario.