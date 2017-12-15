pipeline {
  agent {
    docker {
	image 'atradius_maven:v1'
	registryUrl 'https://ltart001.atradiusnet.com:5001'
	args '-v $HOME/.m2:/root/.m2'
      }
    }
    
  stages {
    stage('build') {
      steps {
        sh 'mvn --version'
        //sh 'mvn -X -v settings.xml -f simple/pom.xml clean package'
        sh 'mvn -X -s settings.xml package'
      }
    }
  }
}
