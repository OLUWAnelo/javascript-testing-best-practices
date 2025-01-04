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

        stage('Log tool') {
          steps {
            echo 'echo "Running tests..."'
          }
        }

      }
    }

    stage('Test') {
      steps {
        sh '''npm install
npm test'''
      }
    }

  }
}