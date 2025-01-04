pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh '''npm init -y
npm install --save-dev jest
test-js.sh'''
      }
    }

  }
}