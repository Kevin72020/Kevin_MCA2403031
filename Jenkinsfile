agent any
stages {
    stage('build') {
        when {
            expression {
                return BRANCH_NAME == 'development' && CODE_CHANGES == true
            }
        }
        steps {
            echo 'building the application...'
        }
    }

    stage('test') {
        when {
            expression {
                return BRANCH_NAME == 'development'
            }
        }
        steps {
            echo 'testing the application...'
        }
    }

    stage('deploy') {
        steps {
            echo 'deploy the application...'
        }
    }
}
