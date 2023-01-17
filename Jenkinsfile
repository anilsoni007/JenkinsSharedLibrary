@Library('AnilShared_lib') _
pipeline {
    agent any
    tools {
  maven 'maven3.8.7'
          }
    stages {
        stage('CheckoutCode') {
            steps {
               git branch: 'main', credentialsId: 'githubid', url: 'https://github.com/anilsoni007/java-web-application.git' 
            }
        }
        stage('Build') {
            steps {
                stages('Build')
            }
        }
        stage('SQ Report') {
             steps {
             stages('SQ Report')
             }
        }
        stage('Nexus') {
           steps {
             stages('Nexus')
           }
        }
    }
}
