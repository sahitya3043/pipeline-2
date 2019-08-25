pipeline {
	agent any
	stages {
		stage('---clean---'){
			steps {
				withMaven(maven: 'maven 3.6.0' mavenSettingsConfig: 'my-maven-settings')
				sh "mvn clean"
			}
		}
	}
}
