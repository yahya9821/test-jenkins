pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh '''npm install -g @angular/cli
ng new test-ci'''
      }
    }

  }
}