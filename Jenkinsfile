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
            
          },
          "test1": {
            build 'test1'
            
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
        parallel(
          "error": {
            sh 'asdfasdfasdf'
            
          },
          "abc": {
            sh 'echo aaaa'
            sh 'echo 123'
            
          },
          "test2": {
            build 'test1'
            
          }
        )
      }
    }
  }
}