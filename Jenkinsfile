pipeline {
    agent any
    stages {
        stage('Build HTML') {
            when {
                changeset "**/*.html"
            }
            steps {
                echo 'Building due to HTML file changes'
            }
        }
    }
}
