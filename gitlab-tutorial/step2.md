There are two options regarding a runner, we can either use a shared runner
or creating our own. Shared runners are often used in smaller projects. 


# Download the Runner
First thing to do is to download the GitLab runner. This can be done with the following command: 
`sudo curl -L --output /usr/local/bin/gitlab-runner "https://gitlab-runner-downloads.s3.amazonaws.com/latest/binaries/gitlab-runner-linux-amd64"`{{execute}}

# Install the Runner
Next step of the runner configuration is to change the access permission in the filesystem. Done simply with the following command: `sudo chmod +x /usr/local/bin/gitlab-runner`{{execute}}


After the permissions have been set, it is required to create a new user to by typing `sudo useradd --comment 'GitLab Runner' --create-home gitlab-runner --shell /bin/bash`{{execute}}


Then to install the runner just execute the following command:  `gitlab-runner install --user=gitlab-runner --working-directory=/home/gitlab-runner`{{execute}}


Lastly, once the installation is complete the runner can be started with `gitlab-runner start`{{execute}}. 
