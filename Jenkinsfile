#!/usr/bin/env groovy
node {
    dir('API-Project') {
        git url: 'https://github.com/snavetrain/API-Project'
    }

    sh('. API-Project/build.sh')
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
                sh 'make check || true'
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
