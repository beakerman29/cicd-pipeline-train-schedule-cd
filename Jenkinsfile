pipeline {
  agent {
    node {
      label 'nginx'
    }

  }
  stages {
    stage('Build') {
      agent {
        node 'CentosTest02'
      }
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts 'dist/trainSchedule.zip'
      }
    }

  }
}