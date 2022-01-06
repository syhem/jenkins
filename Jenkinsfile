pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            sh '''mkdir F1
'''
          }
        }

        stage('ex2') {
          steps {
            sh 'git clone  https://github.com/abesrour1111/git_devops.git'
          }
        }

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
find /home/formation -user formation  > /tmp/formation
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