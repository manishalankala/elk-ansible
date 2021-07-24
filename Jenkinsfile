pipeline {
    agent any
 
    options {
        skipDefaultCheckout(true)
    }
 
    stages {
        stage('Build') {
            steps {
                echo '> Checking out the Git version control ...'
                checkout scm
            }
        }
	stage('Test') {
            steps {
                echo '> Using Super linter'
                
            }
        }
        stage('Deploy') {
            steps {
                echo '> Deploying the application ...'
                ansiblePlaybook(
                    inventory: 'inventory.ini',
                    playbook: 'site.yml'
                )
            }
        }
    }
}
