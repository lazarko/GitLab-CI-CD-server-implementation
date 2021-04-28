GitLab Runner is an application that works with GitLab CI/CD to run jobs in a pipeline

There are three options regarding runners, we can either use shared runners, group runners or specific runners. When choosing which runner you want to use, think about who you want to have access:
- Shared runners are for use by all projects
- Group runners are for all projects and subgroups in a group
- Specific runners are for individual projects

In this tutorial we will show you how to register a specific runner.


# Download the Runner
First thing to do is to download the GitLab runner application. This can be done with the following command: 
`sudo curl -L --output /usr/local/bin/gitlab-runner "https://gitlab-runner-downloads.s3.amazonaws.com/latest/binaries/gitlab-runner-linux-amd64"`{{execute}}

# Install the Runner
Next step of the runner configuration is to change the access permission in the filesystem. Done simply with the following command: `sudo chmod +x /usr/local/bin/gitlab-runner`{{execute}}


After the permissions have been set, it is required to create a new user which is done by typing `sudo useradd --comment 'GitLab Runner' --create-home gitlab-runner --shell /bin/bash`{{execute}}


Then to install the runner just execute the following command:  `gitlab-runner install --user=gitlab-runner --working-directory=/home/gitlab-runner`{{execute}}


Lastly, once the installation is complete the runner can be started with `gitlab-runner start`{{execute}}. 
