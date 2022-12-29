pipeline{
    
    agent any 
    stages {
        
        stage('SSH AGENT'){
            
            steps{
                 sshagent(['ansible_id']) {
                 sudo su - ansadmin;
                 cd /opt;
                 ansible-playbook tomcat_install.yml;
                }
            }
        }    
    }
}
