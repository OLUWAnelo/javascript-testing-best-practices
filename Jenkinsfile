pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git(url: 'https://github.com/OLUWAnelo/javascript-testing-best-practices', branch: 'master')
      }
    }

    stage('Log') {
      steps {
        sh 'ls -la'
      }
    }

    stage('Front-End Test') {
      steps {
        sh 'cd javascript-testing-best-practices-front && npm i && npm run test:unit'
      }
    }

  }
}