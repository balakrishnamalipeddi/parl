pipeline {
    agent none

    stages {
        stage('Build and run') {
          parallel {
            stage('master-agent-pipeline') {
             agent {label 'master'}
              stages{
                stage('Build') {
                steps {
                  echo 'Building on master agent..'
                  }
                }
                stage('Test') {
                  steps {
                    echo 'Testing on master agent..'
                 }
             }
          }
      }
            stage('ubuntu-agent-pipeline') {
             agent{label 'ubuntu'}
              stages{
                stage('Build') {
                steps {
                  echo 'Building on master agent..'
                  }
                }
                stage('Test') {
                  steps {
                    echo 'Testing on master agent..'
                   }
                 }
               }
             }
           }
         }
       }
     }

