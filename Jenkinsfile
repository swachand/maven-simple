pipeline {
    agent any 
    stages {
        stage ('compile stage') { 
            steps{ 
                
                withMaven(maven : 'MVN_3.6.0') { 
                    sh 'mvn clean compile'
                    }
                   
            }
            
        }
        stage ('Testing stage') {
            steps{ 
                
                withMaven(maven : 'MVN_3.6.0') { 
                    sh 'mvn test'
                    }
                   
            }

        }
        stage ('Deployment stage') {
            steps{ 
                
                withMaven(maven : 'MVN_3.6.0') { 
                    sh 'mvn deploy'
                    }
                   
            }

        }
            
    }
}
