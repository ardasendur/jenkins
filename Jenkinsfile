String cron_string = BRANCH_NAME == "master" ? "20 23 * * *" : ""
pipeline {
    agent any
    triggers { cron(cron_string) }
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
       stage('Training') {
            steps {
                echo 'Hello World....'
            }
        }
    }
}
