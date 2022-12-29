pipeline{
    
    agent any 
    stages {
        
        stage('SSH AGENT'){
            
            steps{
                 sshagent(['ansible_id']) {
                     sh 'ssh -o  StrictHostKeyChecking=no ansadmin@52.66.240.134';
                     sh 'sudo su - ansadmin';
                     sh 'cd /opt';
                     sh 'ansible-playbook tomcat_install.yml';
                }
            }
        }    
    }
}
