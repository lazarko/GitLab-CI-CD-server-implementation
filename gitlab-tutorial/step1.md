There are two options regarding a runner, we can either use a shared runner
or creating our own. Shared Runner can be used in smaller projects. 


First what we want to do is to download the GitLab Runner, which can be done with the
following command: `sudo curl -L --output /usr/local/bin/gitlab-runner "https://gitlab-runner-downloads.s3.amazonaws.com/latest/binaries/gitlab-runner-linux-amd64"`


Second part of the Runner pre-installation is to change the access permission in the filesystem of the downloaded object: `sudo chmod +x /usr/local/bin/gitlab-runner`

It is also necessary create a new user to your system with the following command: `sudo useradd --comment 'GitLab Runner' --create-home gitlab-runner --shell /bin/bash`


Now is the time for the Runner installation to the working directory, which is done by invoking: `gitlab-runner install --user=gitlab-runner --working-directory=/home/gitlab-runner`


Once the installation is complete the Runner could be started with just simply `gitlab-runner start`. 


Now we have to register our new Runner to get everything up and running `gitlab-runner register`