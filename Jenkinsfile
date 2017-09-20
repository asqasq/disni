pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        checkout scm
        withMaven( maven: 'Maven', mavenLocalRepo: '.repository') {
          sh "mvn clean install"
        }
     }
  }
}

