pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git 'https://github.com/andreasabipermana/node-api-docker'
      }
    }

    stage('Log') {
      steps {
        sh 'ls -alih'
      }
    }

    stage('Build') {
      steps {
        sh 'docker build -t test .'
      }
    }

  }
}