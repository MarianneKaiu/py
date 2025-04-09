pipeline {
  agent any
  stages {
    stage('build') {
      agent {
        docker {
          image 'python:3'
          reuseNode true
        }
      }
      steps {
        sh '''
        echo "helloww
        '''
      }
    }
  }
}