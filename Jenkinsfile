pipeline {
  agent any
  stages {
    stage('Env& Tools') {
      steps {
        sh 'env'
        sh 'docker --version'
        sh 'ls -ltr'
      }
    }

    stage('Build Dkr') {
      steps {
        sh 'echo \'docker build - t E1Rubens/proyectoCDK:1.0\''
      }
    }

  }
}