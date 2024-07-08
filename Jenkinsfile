pipeline {
    agent any
    stages {
        stage('Build main') {
            when {
                branch 'main'
            }
            steps {
                echo 'Building on main branch'
            }
        }
       stage('Build feature-branch') {
            when {
                branch 'feature-branch'
            }
            steps {
                echo 'Building on main branch'
            }
        }
    }
}
