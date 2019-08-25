pipeline {
	agent any
	stages {
		stage('---clean---'){
			steps {
				 tools { 
       					 maven "maven 3.5.0" 
      					  jdk 'jdk 8u221' 
   					 }
				sh "mvn clean"
			}
		}
	}
}
