pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'git version'
      }
    }

    stage('Test') {
      environment {
        CI = 'true'
      }
      steps {
        sh 'echo "this is test stage."'
      }
    }

  }
}