pipeline {
  agent any
  stages {
    stage('Maven Build') {
      steps {
        sh 'make'
        archiveArtifacts(artifacts: '**/target/*.jar', fingerprint: true)
      }
    }

  }
}