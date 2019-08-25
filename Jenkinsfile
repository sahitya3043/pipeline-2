pipeline {
	agent any
	tools { 
       			maven "maven 3.5.0" 
      			jdk 'jdk 8u221' 
   		}
	stages {
		stage('---clean---'){
			steps {
				sh "mvn clean"
			}
		}
	}
}
