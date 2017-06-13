pipeline {
  agent any
  stages {
    stage('daily') {
      steps {
        parallel(
          "daily": {
            sh 'echo build'
            
          },
          "build2": {
            sh 'echo build2'
            
          }
        )
      }
    }
    stage('deploy') {
      steps {
        sh 'echo no'
      }
    }
    stage('test') {
      steps {
        sh 'echo test'
      }
    }
    stage('error') {
      steps {
        sh 'asdfasdfasdf'
      }
    }
  }
}