pipeline {
    agent any
    tools{ jdk 'jdk 8u221'}
    stages {     
        stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                ''' 
            }
        }
        stage ('Compile Stage') {

            steps {
                withmaven(maven : 'maven3.5.0') {
                    sh "mvn clean compile"
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withmaven(maven : 'maven3.6.1') {
                    sh "mvn test"
                }
            }
        }


        stage ('install Stage') {
            steps {
                withmaven(maven : 'maven3.6.1') {
                    sh "mvn install"
                }
            }
        }
    }
}
