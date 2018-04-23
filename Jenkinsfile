pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Hello'
            sh 'echo 123'
          }
        }
        stage('Test123') {
          steps {
            sh 'echo 4567'
          }
        }
      }
    }
  }
}