Enable email notification on Jenkins
pre-requisites
A Jenkins Server Click here to create
Integration Steps
Log into the Jenkins to install mailer plugin

Install "mailer" plug-in
Manage Jenkins -> Manage Plugins -> available -> mailer
Configure Mailer
Manage Jenkins -> Configure System
E-mail Notification:
SMTP server : smtp.gmail.com
Advanced:
 Use SMTP Authentication
User Name : valaxytech@gmail.com
Passwrod : <password>
 Use SSL
SMTP Port: 465
Charset : UTF-8 (Auto filled)
Unable to authonticate?
please allow your gmail to access "less security apps" click here to enable
Create a Freestyle Project
Create a new job
Job Name : test-email-job
Source code management
Git URL : get URL here
Build Environment
Maven3-Artifactory Integration : `<provide Artifactory server and repository details
`

Build --> Invoke Artifactory Maven3
- Goals:  clean install
Still working
