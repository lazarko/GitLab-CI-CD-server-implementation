# GitLab account

To start off you need to have a GitLab account so if you don't have that yet, go ahead and set it up on [GitLab](https://gitlab.com/users/sign_up)

# Set up a project in GitLab

There are many ways in which you can create projects in GitLab. You can either create a blank project from scratch, import a project from Github, BitBucket, or another source, or even create a project from one of the many templates that GitLab offers. 

The following sections will show you how to set up if you
1. Are starting from scratch and don't have a project
2. Have an existing project in Github

If you already have a project in GitLab you can skip this section and move on to the section `clone project` at the end of this page.

## 1. Set up with a new project

In GitLab, go to Projects -> New project -> Create blank project. Choose a project name and fill out any additional information for your project, and you are all set up!

## 2. Set up with an existing project in GitHub

In GitLab, go to Projects -> New project -> Import project. Click GitHub as the place you want to import your project from. This will redirect you GitHub where you need to agree to authorize access to gitlabhq.

All your repositories from GitHub will now be listed and you can choose which one you want to import. Importing can take a few seconds. Now you are all set up!

# Clone project

Clone your GitLab project using `git clone` with SSH or HTTPS and change diretory to your project using `cd PROJECT_NAME`.