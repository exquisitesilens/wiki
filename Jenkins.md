#Jenkins

[Jenkins]
(http://jenkins-ci.org/) is really very smart to install and configure.
 
My first experience was very good. I have done the follow steps and everything go well: 
 1. Install jenkins-1.530 for Windows (Windows 8) (Java Runtime SE required)
 2. Disable Windows Service "Jenkins", because it does not have sufficient rights to start UI-applications.
 3. Start: 

`cd "c:\Program Files (x86)\Jenkins"`

`java -jar .\jenkins.war`

 4. Install PlugIns MSBuild and EMail ext. and configure them
 5. Add new job: copy new assemblies, build C# solution, copy .exe to the deployment directory finally run the application

Still two problems: 

1. In Post-build Action: Editable Email Notification I can not set "Triggers". After click on "Add Triger" nothing happened?

2. On my Windows 7 Server I can not access as "Login", if I start Jenkins via command line "java -jar jenkins.war"! Error: "HTTP Status 404 - The requested resource () is not available." on http://myserver:8080/jenkins/j_acegi_security_check
I have tried: delete JENKINS_HOME/config.xml, Matrix security and add user, allow all actions and so on.
but it does not help... It maybe relate to [https://issues.jenkins-ci.org/browse/JENKINS-3761](https://issues.jenkins-ci.org/browse/JENKINS-3761)