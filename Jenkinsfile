
pipeline {
    agent {
        label 'maitre'
    }
    stages {
        stage('Build') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'GIT_CREDS', yahya9821: 'USERNAME', podolski98672009: 'PASSWORD')]) {
                    sh "git clone https://${USERNAME}:${PASSWORD}@github.com/yahya9821/test-jenkins.git"
                }
            }
        }
    }
}
