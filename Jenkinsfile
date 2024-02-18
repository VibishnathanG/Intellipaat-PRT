pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git  'https://github.com/VibishnathanG/Intellipaat-PRT.git'
            }
        }

        stage('Run Ansible Playbook') {
            steps {
                script {
                    sh 'ansible-playbook your-playbook.yaml'
                }
            }
        }
    }
}
