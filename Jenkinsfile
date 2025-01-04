pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''bash 
     #!/bin/bash 
     set -e 
     npm install 
     npm build'''
      }
    }

  }
}