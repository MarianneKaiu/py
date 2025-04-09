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
        echo "Jenkins va installer les deps"
        pip install flask
        python index.py
        echo "fin"
        '''
      }
    }
  }
}