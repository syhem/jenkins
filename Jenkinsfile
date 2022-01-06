pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        sh '''mkdir F1
'''
      }
    }

    stage('stage2') {
      steps {
        sh 'grep user /etc/passwd'
      }
    }

    stage('stage 3') {
      steps {
        sh '''if test `grep -c orsys /etc/passwd` -ne 0
then 
find / -user orsys  > /tmp/orsys
fi
'''
      }
    }

    stage('Stage4') {
      steps {
        sh '''For i in `cat /tmp/orsys`
Do
Ls -il $i
done
'''
      }
    }

  }
}