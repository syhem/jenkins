pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        sh '''mkdir F1
'''
      }
    }

    stage('error') {
      steps {
        sh 'sh grep -c \'^username:\' /etc/passwd'
      }
    }

  }
}