node {
    checkout scm (1)
    https://github.com/snavetrain/API-Project.git
}
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'make' (1)
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
    }
}
