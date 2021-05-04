pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the master branch..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing the master branch..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the master branch....'
            }
        }
        stage('Email Notification') {
             steps {
                mail bcc: '', body: '''Hi 
                Email has successfully  sent
                Thanks''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'alok.natheee@gmail.com'
                echo 'Sending email notification....'
            }
        }
    }
}
