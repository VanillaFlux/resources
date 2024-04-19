pipeline {
  agent any
  stages {
    stage('Zip') {
      steps {
        sh 'zip server_resources.zip -r *'
      }
    }

    stage('Archive') {
      steps {
        archiveArtifacts '*.zip'
      }
    }

  }
}