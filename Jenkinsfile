node {
    dir('RepoOne') {
        git url: 'https://github.com/snavetrain/API-Project.git'
    }

    sh('. RepoOne/build.sh')
}
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'make' 
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
