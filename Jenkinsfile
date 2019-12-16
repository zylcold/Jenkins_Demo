pipeline {
  agent any
  stages {
    stage('test') {
      parallel {
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
        stage('build') {
          steps {
            echo 'hhhh'
          }
        }
        stage('deploy') {
          steps {
            echo 'deploy'
          }
        }
      }
    }
    stage('test2') {
      parallel {
        stage('test2') {
          steps {
            echo 'test2'
          }
        }
        stage('build2') {
          steps {
            echo 'build2'
          }
        }
      }
    }
  }
}