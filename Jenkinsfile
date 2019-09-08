pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        sh 'echo "my name is Pranaya"'
        sh '"ls"'
      }
    }
    stage('dev') {
      parallel {
        stage('dev') {
          steps {
            sh 'echo "Test"'
            sh '"ls"'
          }
        }
        stage('sandbox') {
          steps {
            sh 'echo "testing parallel stage"'
          }
        }
      }
    }
    stage('123') {
      steps {
        sh 'echo "test test"'
      }
    }
  }
}