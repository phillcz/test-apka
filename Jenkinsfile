pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'ls -al'
      }
    }
    stage('test1') {
      steps {
        parallel(
          "test1": {
            sleep 5
            
          },
          "test2": {
            sleep 8
            
          },
          "test3": {
            sh '''echo ahoj
false'''
            echo 'xxxx'
            
          }
        )
      }
    }
    stage('konec') {
      steps {
        echo 'konec'
        junit 'xaxa'
      }
    }
  }
  environment {
    aaa = '5'
  }
}