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
        echo 'HHHHHH'
        sleep 5
        sh 'echo \'HHHHH\''
      }
    }
  }
}