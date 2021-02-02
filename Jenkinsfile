#!/usr/bin/env groovy

pipeline {
    agent any
    triggers { pollSCM('* * * * *') }
    stages {
        // implicit checkout stage

        stage('Build') {
            steps {
                sh './mvnw clean package'
            }
        }
    }
}