pipeline {
  agent {
    docker {
	image 'maven:3-alpine'
      }
    }
    
  stages {
    stage('build') {
      steps {
        sh 'mvn -v settings.xml clean package'
      }
    }
  }
}
