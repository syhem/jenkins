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
        sh 'cut -d: -f1,3 /etc/passwd >users'
      }
    }

  }
}