pipeline {
    agent any
    stages{
    
		stage('Build'){
            steps{
            echo 'hi pipeline'
			bat label: '', script: 'mvn clean package'
     
			}
			
			post{
			success{
			archiveArtifacts '**/*.war'
				}
			}
        }
		stage('tomcat'){
            
			steps{
            echo 'hi pipeline2'
			}
               
    	}
		
		stage('test'){
            
			steps{
            echo 'hi pipeline3'
			}
               
    	}
	
	
	
	}
}
