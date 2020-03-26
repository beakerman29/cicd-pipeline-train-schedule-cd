pipeline {
  agent {
    node {
      label 'CentosTest02'
    }

  }
  stages {
    stage('Build') {
      agent {
        node 'CentosTest2'
      }
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts 'dist/trainSchedule.zip'
      }
    }

  }
}