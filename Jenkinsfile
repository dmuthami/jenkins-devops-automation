#!/usr/bin/env groovy

pipeline {

    agent {
        docker {
            image 'node'
            args '-u root'
        }
    }

    stages {
        stage('Build') {
            /* This install the node modules/binaries */
            steps {
                echo 'Building...'
                sh 'npm install'
            }
        }
        stage('Test') {
             /* This builds the actual image */
            steps {
                echo 'Testing...'
                sh 'npm test'
            }
        }
    }
}