pipeline {
  agent {
    node {
      label 'test'
    }
    
  }
  stages {
    stage('build') {
      steps {
        sh 'sudo pip install -r requirments.txt'
      }
    }
    stage('test') {
      steps {
        sh 'pwd'
      }
    }
  }
}