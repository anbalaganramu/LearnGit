pipeline {
    agent none
    environment{
        APP_NAME = 'Pay_Gateway'
    }
    stages {
        stage('Job1') {
            agent {label 'agentSlave'}
            steps {
                withEnv(["version=1.0", "env=prod"]){                    
                     echo "This is version ${version} and environment is ${prod}"
                }
                 echo "It is ${env.JOB_DISPLAY_URL}"
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
