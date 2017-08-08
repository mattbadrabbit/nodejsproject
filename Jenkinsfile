#!/usr/bin/env groovy
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '/root/matt/build.py --repo=file://$WORKSPACE --in-place --flavor=chop-production --customfiles=git@github.com:/BadRabbitCode/os-templates.git --force'
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
