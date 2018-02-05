pipeline {
  agent {
    node {
      label 'dev'
    }
    
  }
  stages {
    stage('git') {
      steps {
        dir(path: '/home/shiyanlou/test_git') {
          git(url: 'git@github.com:yingque/test_git.git', branch: 'master', credentialsId: '2c784d4f-8e18-4f3e-a4e1-45c91795f982')
        }
        
      }
    }
    stage('run') {
      steps {
        dir(path: '/home/shiyanlou/test_git') {
          sh 'python app.py &'
        }
        
      }
    }
  }
}