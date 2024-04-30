pipeline {
    agent any
    stages {
        stage("verifying toolings") {
            steps {
                sh '''
                    docker --version
                    docker-compose --version
                '''
            }
        }
        stage("Starting the container") {
            steps {
                sh 'docker-compose up'
            }
        }
    }
}