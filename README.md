# JenkinsSharedLibrary by Anil Soni
. jenkins shared library is the concept of having a common pipeline code in SCM that can be used by other pipelines as referencing it.

###### Step 1
clone the repository code using 
`git clone https://github.com/anilsoni007/JenkinsSharedLibrary.git`

###### Step 2
Configure the jenkins 
go to 
```
jenkins Dashboard -> manage jenkins -> configure system -> Global Pipeline Libraries
```
Define the jenkins shared library name and mention git hub repo in the jenkins

###### Step 3
to access the shared library in `Jenkinsfile` you need to add @Library annotation.
`@Library('AnilShared_lib') _ `
