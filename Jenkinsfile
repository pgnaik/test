pipeline {
    agent any
    stages {
        stage('Test') {
            when {
                environment name: 'RUN_TESTS', value: 'true'
            }
            steps {
                echo 'Running tests'
            }
        }
    }
