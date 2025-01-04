pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh '''  #!/bin/bash 
     set -e 
     npm install 
     npm test '''
      }
    }

  }
}