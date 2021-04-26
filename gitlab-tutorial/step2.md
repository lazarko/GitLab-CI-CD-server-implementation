Now that we have downloaded and installed our Runner we need to link it to a GitLab repository. 
Head on to the GitLab site and chose whether you are going to create a project from scratch or import an already existing one.   
Once the project has been chosen head to the settings and click on `CI/CD` as shown in the image below. 
![Find Settings Image](https://github.com/lazarko/GitLab-CI-CD-server-implementation/blob/main/resources/images/register_runner_1.png)

When you are in the CI/CD go to the Runner (click on expand) and you will get the following information that you are going to copy.
![Find Runner Register Image](https://github.com/lazarko/GitLab-CI-CD-server-implementation/blob/main/resources/images/register_runner_2.png)




Now we have to register our new Runner to get everything up and running `gitlab-runner register`{{execute}} and add the information 
that you have copied. 








Next step is to create a YAML file, which will set the foundation of the CI/CD server. 