pipeline {
    agent any

    stages {
        stage('Checkout Jenkinsfile') {
            steps {
                git branch: 'main', credentialsId: '558deb00-7e56-4f7d-8cc5-bddac97400f2', url: 'https://github.com/VibishnathanG/Intellipaat-PRT.git'
            }
        }

        stage('Ansible install web Application') { 
            steps {
                
                sh 'sudo ansible-playbook webinstall_playbook.yaml' 
            }
        }
    }
}
