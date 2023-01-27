pipeline {
  agent {
      label 'maitre'
  }
  stages {
    stage('Initialization') {
      steps {
        sh 'npm install -g @angular/cli'
        sh 'ng new test-ci'
      }
    }

    stage('Build') {
      steps {
        sh 'cd test-ci'
        sh 'ng build --prod'
      }
    }

    stage('Test') {
      steps {
        sh 'cd test-ci'
        sh 'ng test'
      }
    }

    stage('Deploy') {
      steps {
        sh 'cd test-ci'
        sh 'ng deploy --prod'
      }
    }

  }
  environment {
    PATH = "${tool 'node'}/bin:${env.PATH}"
  }
}
