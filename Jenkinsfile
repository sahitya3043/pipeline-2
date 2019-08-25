pipeline {
	agent any
	stages {
		stage('---clean---'){
			steps {
				withMaven(maven:'maven 3.6.0')
				sh "mvn clean"
			}
		}
		stage('---test---') {
			steps {
				withMaven(maven:'maven 3.5.0')
				sh "mvn test"
			}
		}
		stage('---package---'){
			steps {
				withMaven(maven:'maven3.3.3')
				sh "mvn package"
			}
		}
	}
}
