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
            sh 'false'
            
          }
        )
      }
    }
    stage('konec') {
      steps {
        echo 'konec'
      }
    }
  }
  environment {
    aaa = '5'
  }
}