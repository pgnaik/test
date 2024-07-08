pipeline {
    agent any
    environment {
        RUN_TESTS = 'true'
       DEPLOY = 'false'
    }
    stages {
        stage('Build') {
            when {
                branch 'main'
            }
            steps {
                echo 'Building on main branch'
            }
        }
        stage('Test') {
            when {
                environment name: 'RUN_TESTS', value: 'true'
            }
            steps {
                echo 'Running tests'
            }
        }
        stage('Deploy') {
            when {
                allOf {
                    branch 'main'
                    expression {
                        return env.DEPLOY == 'true'
                    }
                }
            }
            steps {
                echo 'Deploying to production'
            }
        }
    }
}
