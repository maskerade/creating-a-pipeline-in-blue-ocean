pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'ls -ls'
            echo 'Build Complete'
          }
        }
        stage('Parallel Build1') {
          steps {
            echo 'Parallel Build3 Complete'
          }
        }
        stage('Parallel Build2') {
          steps {
            echo 'Parallel Build3 Complete'
          }
        }
        stage('Parallel Build3') {
          steps {
            echo 'Parallel Build3 Complete'
          }
        }
      }
    }
    stage('Test') {
      steps {
        echo 'Tests Complete'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy Complete'
      }
    }
  }
  environment {
    test = '1'
  }
}