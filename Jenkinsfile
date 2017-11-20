pipeline {
  agent {
    docker {
	image 'maven:3-alpine'
      }
    }
    
  stages {
    stage('build') {
      steps {
        sh 'mvn -x -v settings.xml clean package'
      }
    }
  }
}
