pipeline {
  agent any
  stages {
    stage('daily') {
      steps {
        build 'build1'
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
  }
}