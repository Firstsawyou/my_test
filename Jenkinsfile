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
        sh './jenkins/scripts/test.sh'
      }
    }

  }
}