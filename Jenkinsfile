pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        parallel(
          "bb": {
            sh 'a'
            
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
      }
    }
  }
}