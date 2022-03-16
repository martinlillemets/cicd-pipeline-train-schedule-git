pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                echo 'Building app with gradle'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
