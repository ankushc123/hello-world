pipeline{
      environment {
    /*
     define your command in variable
     */
    remoteCommands =
      """
                     sh 'cd /opt'
                     sh 'ansible-playbook tomcat_install.yml'
      """
  }
   stages{
        stage('Git CheckOut')
        {
            steps{
                script{
                 git 'https://github.com/ankushc123/hello-world.git'
                }
            }
        }        
  /*      stage('SSH AGENT'){
            
            steps{
                 sshagent(['ansadmin-id']) {
                     script 
                            {
                               sh """ssh -tt ansadmin@52.66.240.134 -o StrictHostKeyChecking=no $remoteCommands 
                            }
                }
            } */
        }       
}
