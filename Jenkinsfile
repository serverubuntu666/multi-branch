pipeline {
    agent { label 'DEV'}
    environment {
        branch_name = 'feature'
    }

    stages {
        stage ('build') {
            steps {
                sh 'echo "This build is on main ${branch_name}."'
            }
        }

        stage ('test') {
            steps {
                sh 'echo "This test is on ${branch_name}.'
            }
        }

        stage ('deploy') {
            steps {
                sh 'echo "This deploy is on ${branch_name}.'
            }
        }
    }
}
