pipeline{
	agent{
		docker{
			image 'maven:3-alpine'
			args '-v /root/.m2:/root/.m2 -v /home/settings.xml:/usr/share/maven/conf/settings.xml'
		}
	}
	stages{
		stage('Build'){
			steps{
				sh 'mvn -version'
			}
		}
	}
}
