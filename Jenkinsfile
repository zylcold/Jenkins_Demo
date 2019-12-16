pipeline {
  agent {
    node {
      label 'ios'
    }

  }
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
            echo 'HHHHHH'
            sleep 5
          }
        }
        stage('build') {
          agent {
            node {
              label 'ios'
            }

          }
          steps {
            echo 'hhhh'
          }
        }
        stage('deploy') {
          agent {
            node {
              label 'ios'
            }

          }
          steps {
            echo 'deploy'
          }
        }
      }
    }
    stage('test2') {
      parallel {
        stage('test2') {
          agent {
            node {
              label 'ios'
            }

          }
          steps {
            echo 'test2'
          }
        }
        stage('build2') {
          agent {
            node {
              label 'ios'
            }

          }
          steps {
            echo 'build2'
          }
        }
      }
    }
  }
}