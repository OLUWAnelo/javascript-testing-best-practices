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

    stage('GIT LOGIN') {
      environment {
        GITHUB_USER = 'DevOps4321'
        GITHUB_PASSWORD = 'OLUWAnelo'
      }
      steps {
        sh 'git login -u $GITHUB_USER -p $GITHUB_PASSWORD '
      }
    }

  }
}