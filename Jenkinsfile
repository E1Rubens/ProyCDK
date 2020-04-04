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
        sh 'docker build -t e1rubs/conexion:v6 .'
        sh 'docker images'
      }
    }

    stage('Push Dkr') {
      steps {
        sh 'docker push e1rubs/conexion:v6'
      }
    }

  }
}