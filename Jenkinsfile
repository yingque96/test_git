pipeline {
  agent {
    node {
      label 'test1'
    }
    
  }
  stages {
    stage('build') {
      steps {
        dir(path: '/home/shiyanlou/shiyanlou')
        git(url: 'https://github.com/yingque/test_git.git', branch: 'master', credentialsId: 'ed1c0023-a806-4a1c-a5ce-878280818ca7')
      }
    }
    stage('test') {
      steps {
        sh 'pwd'
        dir(path: '/home/shiyanlou/shiyanlou') {
          sh 'python app.py'
        }
        
      }
    }
  }
}