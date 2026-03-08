pipeline {
    agent none
    environment{
        APP_NAME = 'Pay_Gateway'
    }
    stages {
        stage('Job1') {
            agent {label 'agentSlave'}
            steps {
                echo "Welcome to ${APP_NAME} application."
            }
        }
        stage('Job2') {
            agent any
            steps {
                echo 'This is Job2'
            }
        }        
    }
}
