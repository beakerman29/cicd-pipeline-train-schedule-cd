pipeline {
    agent any
    stages {
        stage('Build') {
            agent { 
                node('CentosTest2')
            }
            steps {
                echo 'Running build automation'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}