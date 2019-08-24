pipeline {
    agent any
    tools{ jdk 'jdk 8u221'}
    stages {
        stage ('Compile Stage') {

            steps {
                withmaven(maven : 'maven3.6.1') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withmaven(maven : 'maven3.6.1') {
                    sh 'mvn test'
                }
            }
        }


        stage ('install Stage') {
            steps {
                withmaven(maven : 'maven3.6.1') {
                    sh 'mvn install'
                }
            }
        }
    }
}
