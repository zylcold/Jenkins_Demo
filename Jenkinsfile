pipeline {
  agent any
  stages {
    stage('test') {
      agent {
        node {
          label 'ios'
        }

      }
      steps {
        sh 'echo "Hello"'
      }
    }
  }
}