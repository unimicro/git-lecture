#!/usr/bin/env groovy

pipeline {
    agent any

    stages {
        stage('Setup') {
            steps {
                echo 'Setup...'
                bat 'yarn install'
            }
        }
        stage('Build') {
            steps {
                echo 'Build...'
                bat 'yarn build.dev'
            }
        }
        stage('Package') {
            steps {
                echo 'Package...'
                bat 'yarn zip-dist'
            }
        }
    }
}
