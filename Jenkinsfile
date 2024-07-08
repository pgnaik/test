pipeline {
    agent any
    stages {
        stage('Deploy') {
            when {
                expression {
                    return env.BRANCH_NAME == 'main' && currentBuild.result == null
                }
            }
            steps {
                echo 'Deploying on main branch'
            }
        }
    }
}
