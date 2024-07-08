pipeline {
    agent any
    environment {
        RUN_TESTS = 'false'
    }
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
}
