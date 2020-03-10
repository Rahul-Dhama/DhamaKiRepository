pipeline {

	agent any
	tools {
        maven 'Maven_3.5.2' 
    	}
	stages{
		stage('Compile Stage'){
		steps{
				withMaven(maven : 'Maven'){
					sh 'mvn clean compile'
				}		
			}
		}
			stage('Testing Stage'){
			steps{
				withMaven(maven : 'Maven'){
					sh 'mvn test'
				}		
				}
			}
			
			stage('Deployment Stage'){
			steps{
				withMaven(maven : 'Maven'){
					sh 'mvn deploy'
				}		
				}
			}
			
		}
	
}
