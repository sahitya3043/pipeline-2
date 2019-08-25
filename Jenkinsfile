pipeline {
	agent any
	stages {
		stage('---clean---'){
			withMaven(maven:'maven 3.6.0')
			steps {
				sh "mvn clean"
			}
		}
		stage('---test---') {
			withMaven(maven:'maven 3.5.0')
			steps {
				sh "mvn test"
			}
		}
		stage('---package---'){
			withMaven(maven:'maven3.3.3')
			steps {
				sh "mvn package"
			}
		}
	}
}
