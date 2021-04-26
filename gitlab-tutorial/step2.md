Now that we have downloaded and installed our Runner we need to link it to a GitLab repository. 
Head on to the GitLab site and chose whether you are going to create a project from scratch or import an already existing one.   
Once the project has been chosen head to the settings and click on `CI/CD` as shown in the image below. 
![Find Settings Image](/Users/Lazarko/PycharmProjects/GitLab-CI-CD-server-implementation/assets/register_runner_1.png)

When you are in the CI/CD go to the Runner (click on expand) and you will get the following information that you are going to copy.
![Find Runner Register Image](/Users/Lazarko/PycharmProjects/GitLab-CI-CD-server-implementation/assets/register_runner_2.png)




Now we have to register our new Runner to get everything up and running `gitlab-runner register`{{execute}}.
1. Add the URL from GitLab and press enter.
2. After adding URL, copy the token and paste it in the terminal. 
2. Next, add description for the runner. This can be changed later on in the GitLab UI.
3. The terminal will then ask you to enter the tags associated with the runner, right now 
you can just press enter. Don't worry this can be changed later on in the GitLab UI.
4. Now you have an option to choose a runner executor. For the sake of this tutorial just write shell and press enter to continue.
After everything is completed refresh the GitLab page and you will see the new runner, like in the image below.
   
![Find Runner Register Image](/Users/Lazarko/PycharmProjects/GitLab-CI-CD-server-implementation/assets/runner_running.png)
   