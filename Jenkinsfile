pipeline {
  agent {
    docker {
	image 'maven:3-alpine'
	args '-v $HOME/.m2:/root/.m2'
      }
    }
    
  stages {
    stage('build') {
      steps {
        sh 'mvn --version'
        //sh 'mvn -X -v settings.xml -f simple/pom.xml clean package'
        sh 'mvn -X -s settings.xml clean package'
      }
    }
  }
}
