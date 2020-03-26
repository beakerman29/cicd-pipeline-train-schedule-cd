pipeline {
<<<<<<< HEAD
    agent none
    stages {
        stage('Build') {
            agent {
                node('CentosTest02')
            } 
            steps {
                echo 'Running build automation'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
=======
  agent {
    node {
      label 'CentosTest02'
>>>>>>> b3fbeda52f3510e023901b3d93ee0feaf56181bd
    }

  }
  stages {
    stage('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts 'dist/trainSchedule.zip'
      }
    }

  }
}