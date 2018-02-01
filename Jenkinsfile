pipeline {
  agent {
    node {
      label 'test'
    }
    
  }
  stages {
    stage('build') {
      steps {
        dir(path: '/home/shiyanlou') {
          git(url: 'https://github.com/yinqgue/test_git.git', branch: 'master', credentialsId: '92d7b501-5ee9-4997-a38d-4150208ac5ae')
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