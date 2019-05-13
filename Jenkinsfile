pipeline {
    agent any
	
	parameters {
		string (name: 'gitName' , default value : 'mr.jenkins', description :'who should i say hello to')
		text (name: 'biography' ,default value: 'vinitha', description: 'enter some info about the person')
		booleanParam(name:'toogle', default value: true ,description : 'toogle this value')
		choice (name:'my param', choices : "option1\noption2\noption3\n" , description: 'delimters within the string')
		password (name : 'password' , default value: 'secret' , description: 'enter password')
		file (name: 'file', default value: '' , description: 'choose a file')
	
	}
	
    stages{
    
		stage('Build'){
            steps{
            echo 'hi pipeline'
			echo "hello $(params.Person)
			echo "biography: $(params.biography)
			echo "toog: $(params.toogle)
			
     
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
