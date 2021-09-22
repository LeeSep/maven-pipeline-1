#!/usr/bin/env groovy

pipeline {
    agent any

    tools {
        maven 'mvn-3.5.4'
        jdk 'jdk-8u181'
    }

    stages {
        stage('Build') {
            steps {
                sh "printenv"
                sh "mvn clean test package spring-boot:repackage"

            }
        }
}
