pipeline {
	agent any
	stages {
		stage('---clean---'){
			steps {
				withMaven('maven 3.6.0')
				sh "mvn clean"
			}
		}
	}
}
