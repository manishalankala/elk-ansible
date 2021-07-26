pipeline {
    agent any
 
 
    stages {
        stage('Build') {
            steps {
                echo '> Checking out the Git version control ...'
                checkout scm
            }
        }
	stage('Test') {
            steps {
                echo '> Using ansible-lint'
		sh 'apt install python3'
		sh 'apt-get install python -y'
		sh 'apt-get install ansible -y'
                sh 'pip3 install "ansible-lint[yamllint]"'
		sh 'ansible-lint'
		sh 'ansible-galaxy collection install ansible.posix'
		sh 'ansible-galaxy collection install community.docker'
		
                
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
