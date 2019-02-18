pipeline {
  agent any
  stages {
    stage('Build') {
<<<<<<< HEAD
      steps {
        sh 'echo "build"' asfasfasfasfas
=======
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
>>>>>>> d67a0993c761b74c8ab23c152bf2b01454f0c737
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
