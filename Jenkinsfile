pipeline {
    agent any
    stages {
        stage ('Echo') {
            steps {
                echo 'running build automation on the Master node'
            }

            steps ('Build') {
            sh './gradlew build --no-daemon'
            archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }

    }
}
