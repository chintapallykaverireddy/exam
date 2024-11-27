pipeline {
  agent any 
    stages {
      stage('build') {
        steps {
          script {
            bat "docker build -t exam ."
            bat "docker run -d -p 3000:3000 exam:latest"
          }
        }
      }
      stage('run'){
        steps {
          script {
            echo "runni"
          }
        }
      }
      stage('test'){
        steps{
          script {
            echo "testing"
          }
        }
      }
    }
  }
  
