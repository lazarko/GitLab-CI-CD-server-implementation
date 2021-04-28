# Add, Commit and Push Changes
Prepare all the files before the commit using `git add --all`{{execute}}. 

Next stage is to commit the changes by doing the `git commit -m "test CI/CD server"`{{execute}}.

Git might ask you to register as a user. If so, enter `git config --global user.email "you@example.com"`, with your email and try to commit again.

Lastly, just push the changes with `git push`{{execute}} command. If you created an empty project you might need to use the `git push -u origin master`{{execute}} command instead.

# Check the status of your pipeline

In your project go to CI/CD. You should see your pipeline at the top of the page and by clicking on the pipeline id you can see a visual representation of the pipeline. 

If everything works and all stages pass, congrats you have a working CI/CD pipeline and you can now alter the `.gitlab-ci.yml` file to fit your project.

If any of the stages fail, look at the next section.

# Caveat!
Observe that the version of Git may be outdated on Katacoda.
In the case that this causes problems, try using following commands to fix the issue: 


1. Remove the old version of git with: `sudo yum remove git`{{execute}}. When promted, type "y".

2. Download the new version of git: `sudo yum install -y https://repo.ius.io/ius-release-el7.rpm`{{execute}}.

3. Install the new downloaded version `sudo yum install git222`{{execute}}. When promted, type "y".

4. Run `git --version`{{execute}} to control that the right version is installed (git version 2.22.5).

5. Commit using the command `git commit -m "second test CI/CD server" --allow-empty`{{execute}} and then `git push`{{execute}}.

6. Check your pipeline again and it should pass all stages!