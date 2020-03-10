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
		   def mvnHome =tool name: 'Maven', type: 'maven'
			sh "${mvnHome}/bin/mvn package"
			}
		}
	}		
	
}
