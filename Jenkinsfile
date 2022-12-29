pipeline{
    
    agent any 
    stages {
        
        stage('SSH AGENT'){
            
            steps{
                 sshagent(['ansible']) {
                 sudo su - ansadmin;
                 cd /opt;
                 ansible-playbook tomcat_install.yml;
                }
            }
        }    
    }
}
