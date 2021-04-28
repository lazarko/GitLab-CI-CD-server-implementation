
# Check GitLab Settings
Go to the project on GitLab and navigate to the `Settings`. From the settings click on `CI/CD` as shown in the image below. 
![Find Settings Image](./assets/register_runner_1.png)

When you are in the CI/CD section go to the Runner by clicking on expand. From there you will find **your** URL and token, which are used in the second part of the registration. Do not use the ones in the image as these won't work for your project.
![Find Runner Register Image](./assets/register_runner_2.png)

# Register the Runner 
Now it is time to make GitLab aware of our new runner. Run the following command: `gitlab-runner register`{{execute}} and do the following:
1. Add the URL from GitLab and press enter.
2. After adding URL, copy the token and paste it in the terminal. 
2. Next, add description for the runner. This can be changed later on in the GitLab UI.
3. The terminal will then ask you to enter the tags associated with the runner, right now you can just press enter. Don't worry this can be changed later on in the GitLab UI. Tags are used so that when a CI/CD job runs, it knows which runner to use by looking at the assigned tags. This allows you to have specific runners for different stages of your pipeline.
4. Now you have an option to choose a runner executor. An executor determines the environment each job runs in. For the sake of this tutorial we will write shell since this will depend on your project. Press enter to continue.
After everything is completed, refresh the GitLab page and you will see the new runner (see image below).
   
![Find Runner Register Image](./assets/runner_running.png)
   