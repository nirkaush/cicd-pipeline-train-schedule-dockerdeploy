pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh 'gradle build --no-daemon'
                sh 'echo $PATH'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
