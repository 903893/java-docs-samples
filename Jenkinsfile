pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo "hello world"'
      }
    }
    stage('test') {
      steps {
        retry(count: 3) {
          dir(path: '/var')
        }
        
      }
    }
    stage('post') {
      steps {
        echo 'tesr'
      }
    }
  }
}