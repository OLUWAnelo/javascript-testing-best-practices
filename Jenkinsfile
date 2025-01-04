pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git(url: 'https://github.com/OLUWAnelo/javascript-testing-best-practices', branch: 'master')
      }
    }

    stage('Log') {
      parallel {
        stage('Log') {
          steps {
            echo '"Starting JavaScript test pipeline..."'
          }
        }

        stage('Npm Test') {
          steps {
            sh '''cd javascript-testing-best-practices-front && npm i && npm run test:unit
'''
          }
        }

      }
    }

  }
}