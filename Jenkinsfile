pipeline {
    agent any

    
    stages {
        stage('Build') {
            steps {
               
                git 'https://github.com/sakthinatural/ansible-nagios-ubuntu.git'
                
                
                ansiblePlaybook credentialsId: 'remote-server', disableHostKeyChecking: true, installation: 'ansible', inventory: 'hosts', playbook: 'install/nagios.yml'
             
            }

            
        }
    }
}
