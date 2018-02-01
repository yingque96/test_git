pipeline {
  agent {
    docker {
      image 'python:2.7'
      args '-p 1000:1000'
    }
    
  }
  stages {
    stage('build') {
      steps {
        sh '''pip install -r requirments.txt
&& pwd'''
      }
    }
  }
}