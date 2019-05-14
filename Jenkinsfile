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
			echo 'archived'
				}
			}
        }
		
		
		stage('deploy to tomcat'){

			steps{

			build 'pipeline2_helloworld_job2_deploytomcat'


			}


		}
	
	
	
	}
}
