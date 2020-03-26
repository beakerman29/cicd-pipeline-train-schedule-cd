pipeline {
  agent none

  }
  stages {
    stage('Build') {
      node('CentosTest02')
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts 'dist/trainSchedule.zip'
      }
    }

  }
}