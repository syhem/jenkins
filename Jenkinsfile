pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        sh '''sh "date"
sh "mkdir F1"
'''
      }
    }

    stage('') {
      steps {
        sh 'sh grep -c \'^username:\' /etc/passwd'
      }
    }

  }
}