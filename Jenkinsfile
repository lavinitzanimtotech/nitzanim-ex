/* Requires the Docker Pipeline plugin */
post {
    always {
        script { 
            ng-container.stop()
        }
    }
}
pipeline {
    agent { docker { image 'python:3.12-rc-bullseye' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
    }
}
