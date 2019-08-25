pipeline {
	agent any
	stages {
		stage('---clean---'){
			steps {
				withMaven(maven: [maven 3.6.0])
				sh "mvn clean"
			}
		}
	}
}
