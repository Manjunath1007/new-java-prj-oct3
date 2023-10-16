pipeline {
    agent any 
    stages{
        stage ('clone') {
            steps {
                git url: 'https://github.com/Manjunath1007/new-java-prj-oct3.git', branch: 'main'
                
                
            }
            
        }
        
        
        stage ('build') {
            steps {
               
                sh 'mvn clean install'
                
            }
            
        }
        
        
        stage ('deploy') {
            steps {
               
                sh 'sudo cp target/*.war /home/ec2-user/apache-tomcat-10.1.13/webapps'
                
            }
            
        }
        
        
 }
}
