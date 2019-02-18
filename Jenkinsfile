pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "build"'
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
