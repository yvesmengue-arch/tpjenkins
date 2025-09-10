pipeline {
  agent any
  stages {
    stage('stage 1') {
      steps {
        sh '''date
'''
      }
    }

    stage('stage 2') {
      steps {
        sh 'dpkg -l > /tmp/paquets'
      }
    }

    stage('stage 3') {
      steps {
        sh '''if test `grep -c user /etc/passwd` -ne 0
then
find / -user user > /tmp/user
fi'''
      }
    }

  }
}