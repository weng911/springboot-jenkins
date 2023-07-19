pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean install'
      }
    }

    stage('Achieve') {
      steps {
        archiveArtifacts 'target/*.jar'
      }
    }

  }
}