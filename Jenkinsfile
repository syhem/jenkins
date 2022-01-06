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
        sh '''if test `grep -c formation /etc/passwd` -ne 0
then 
find /home/formation -user orsys  > /tmp/formation
fi
'''
      }
    }

    stage('Stage4') {
      steps {
        sh '''for i in `cat /tmp/orsys`
do
ls -il $i
done
'''
      }
    }

  }
}