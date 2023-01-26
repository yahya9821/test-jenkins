pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh 'ng test --watch'
      }
    }

    stage('Build') {
      steps {
        sh '''npm install
ng build'''
      }
    }

    stage('Deploy') {
      steps {
        sh 'echo "hello world"'
      }
    }

  }
}