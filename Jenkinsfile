pipeline {
  agent {
    docker {
	image 'maven:3-alpine'
      }
    }
    
  stages {
    stage('build') {
      steps {
        sh 'mvn -X -v settings.xml clean package'
      }
    }
  }
}
