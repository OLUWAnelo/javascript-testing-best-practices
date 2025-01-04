pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git(url: 'https://github.com/OLUWAnelo/javascript-testing-best-practices', branch: 'master')
      }
    }

    stage('Build') {
      steps {
        sh '''npm install
npm test'''
      }
    }

  }
}