pipeline {
  agent any
  tools {
    withMaven(mavenOpts: MAVEN_OPTS, maven: 'M3', mavenLocalRepo: MAVEN_LOCAL_REPOSITORY, mavenSettingsConfig: MAVEN_SETTINGS) {
    sh "mvn ..."
    maven 'M3'
  }
  stages {
    stage('Build') {
      steps {
        sh 'mvn -B -DskipTests clean package'
      }
    }
  }
}
}
