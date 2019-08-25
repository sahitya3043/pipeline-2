pipeline {
	agent any
	stages {
		stage('---clean---'){
			steps {
				tool name: 'maven 3.6.0', type: 'maven'
				sh "mvn clean"
			}
		}
	}
}
