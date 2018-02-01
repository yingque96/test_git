pipeline {
  agent {
    node {
      label 'test'
    }
    
  }
  stages {
    stage('build') {
      steps {
        dir(path: '/home/shiyanlou/shiyanlou') {
          sh 'pwd'
        }
        
      }
    }
    stage('test') {
      steps {
        sh 'pwd'
      }
    }
  }
}