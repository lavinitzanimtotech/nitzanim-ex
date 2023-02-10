/* 
Docker Pipeline plugin */

pipeline {
    agent { docker { image 'python:3.12-rc-bullseye' } }
    stages {
        stage('build') {
            steps {
                sh 'docker build /home/ec2-user/flaskapp/nitzanim-ex/nitzanim-ex'
            }
        }

        stage('')
    }
}
