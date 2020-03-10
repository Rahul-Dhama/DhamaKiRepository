pipeline {

	agent any
	stages{
		stage('SCM Checkout'){
			steps{
		   git 'https://github.com/Rahul-Dhama/DhamaKiRepository'
			}
		}
		stage('Compile-Package'){
			steps{
		   
			sh 'mvn clean install'
			}
		}
	}		
	
}
