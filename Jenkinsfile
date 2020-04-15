pipeline {
    agent any 
    stages {
        stage ('Compile stage') { 
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
        stage ('Install stage') {
            steps{ 
                
                withMaven(maven : 'MVN_3.6.0') { 
                    sh 'mvn install'
                    }
                   
            }

        }
            
    }
}
