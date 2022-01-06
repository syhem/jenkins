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
        sh 'cut -d: -f1,3 /etc/passwd >users'
      }
    }

    stage('stage 3') {
      steps {
        sh '''id_prim_groups=`cut -d: -f4 /etc/passwd`
for i in $id_prim_groups
do
grep $i /etc/group | cut -d: -f1 >>f1
done'''
      }
    }

  }
}