#!/usr/bin/groovy
pipeline {
    agent none

    stages {
        stage('Testing') {
            agent {
                docker {
                    image 'quay.io/ansible/molecule'
                }
            }
            steps {
                dir('roles/bootstrap') {
                    sh 'molecule test'
                }
            }
        }
    }
}
