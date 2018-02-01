pipeline {
  agent {
    docker {
      image 'python:2.7'
      args '-p 8001:8001'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        sh 'pip install -r requirments.txt'
      }
    }
    stage('Test') {
      steps {
        sh 'echo "test suc"'
      }
    }
    stage('Deliver') {
      steps {
        sh 'echo "end del"'
      }
    }
  }
}