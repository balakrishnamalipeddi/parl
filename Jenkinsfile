pipeline {
    agent none

    stages {
        stage('Build and run') {
          parallel {
            stage('master-agent-pipeline') {
              stages{
                stage('Build') {
                steps {
                  echo 'Building..'
                  }
                }
                stage('Test') {
                  steps {
                    echo 'Testing..'
                 }
                }
      }
              }
            stage('ubuntu-agent-pipeline') {
              stages{
                stage('Build') {
                steps {
                  echo 'Building..'
                  }
                }
                stage('Test') {
                  steps {
                    echo 'Testing..'
                 }
                }
               }
              }
             }
            }
           }
          }

