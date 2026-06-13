pipeline {
    agent any
    stages {

        stage('Clone Repository') {
            steps {
                git branch: 'master',
                url: 'https://github.com/swap115/ansible-jenkins-lab.git'
            }
        }
        stage('Run Ansible Playbook') {
            steps {
                sh 'ansible-playbook -i hosts install_apache.yml'
            }
        }
    }
}
