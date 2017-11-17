pipeline {
  agent {
    docker {
      image 'jenkins/ssh-slave:latest'
    }
    
  }
  stages {
    stage('build') {
      steps {
        sh 'cat /etc/hostname'
      }
    }
  }
}