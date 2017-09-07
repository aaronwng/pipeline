pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        parallel(
          "bb": {
            sh 'ls -al'
            
          },
          "aaa": {
            sh 'ls'
            
          }
        )
      }
    }
    stage('bb') {
      steps {
        sh 'ls'
        echo 'hello'
      }
    }
  }
}