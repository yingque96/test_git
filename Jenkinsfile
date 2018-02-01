pipeline {
  agent {
    node {
      label 'test'
    }
    
  }
  stages {
    stage('build') {
      steps {
        sh 'pip install -r requirments.txt'
      }
    }
    stage('test') {
      steps {
        sh 'pwd'
      }
    }
  }
}