pipeline {
  agent any
  stages {
    stage('error') {
      parallel {
        stage('bb') {
          steps {
            sh 'ls -al'
          }
        }
        stage('aaa') {
          steps {
            sh 'ls'
          }
        }
      }
    }
    stage('bb') {
      agent {
        docker {
          image 'ubuntu'
        }
        
      }
      steps {
        sh 'ls'
        echo 'hello'
      }
    }
  }
}