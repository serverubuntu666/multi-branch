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
                sh 'echo "This test is on ${branch_name}."'
                // sh 'ansible-playbook /mnt/d/drivef/devops/practice-ansible/playbooks/06-stdout.yml'
            }
        }

        stage ('deploy') {
            steps {
                sh 'echo "This deployment is on ${branch_name}."'
            }
        }
    }
}
