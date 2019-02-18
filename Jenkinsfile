pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'echo "build step"'
          }
        }
        stage('paral') {
          steps {
            echo 'parallel'
          }
        }
        stage('paral2') {
          steps {
            retry(count: 3) {
              echo 'paral2'
            }

          }
        }
        stage('') {
          steps {
            sh 'python test.py'
          }
        }
      }
    }
    stage('Test') {
      steps {
        echo 'test step'
      }
    }
    stage('deploy') {
      steps {
        sh 'echo "deploy step"'
      }
    }
  }
}