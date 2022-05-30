# automated-webserver-setup-with-jenkins-and-git

In this project I have created a automated pipeline for Apache webserver deployment. This pipeline is connected to the GitHub repository, so any change in the repository will be automatically detected and accordingly the webpage automatically gets modified. 

### Tool and Technology  used
* Git
* Jenkins
* Redhat Linux
* HTML & CSS
* Apache httpd webserver


## Trigger used for Auto change Detection
In Jenkins, I used Poll SCM trigger which will go to github repo in every 1 minute (60 sec) and if there is any change is commit id than that of previous then it triggers it and pull the changed code and build it.

## automated push from local github to Global GitHub repository
To make automated push as any commit done in the local workspace, I used a post-coomit hook. This script run automatically as any commit done and code is being uploaded in automated way and then i will automatically detected by Jenkins.
