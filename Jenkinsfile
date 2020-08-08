pipeline{
    
    agent any
    tools{
        
        maven 'mymaven'
        jdk 'myjava'
    }
    
    stages{
        stage('gitcheckout'){
            steps{
                
                git 'https://github.com/devopsstephen/warrepo.git'
            }
        }
          
          stage('package'){
              
              steps{
                  
                  sh 'mvn clean package'
              }
          }
    }
}
