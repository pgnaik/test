pipeline {
    agent any
       environment {
        RUN_BUILD = 'true'
    }
    stages {
        stage('Build and Test') {
            when {
                allOf {
                    branch 'main'
                    environment name: 'RUN_BUILD', value: 'true'
                }
            }
            steps {
                echo 'Building and testing on main branch'
            }
        }
    }
}
