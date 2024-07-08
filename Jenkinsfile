pipeline {
    agent any
    environment {
        RUN_TESTS = 'true'
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
