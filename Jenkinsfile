pipeline{
    
    agent any 
    environment {
    PATH="/opt/apache-maven-3.8.6/bin:$PATH"
    }
    
    stages {
        
        stage('Git Checkout'){
            
            steps{

                    git branch: 'main', url: 'https://github.com/ankushc123/demo-counter-app.git'

            }
        }    
        stage('maven compile'){
            
            steps{
                    
                   sh 'mvn compile'
            }
        }       
}
}
