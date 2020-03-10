pipeline {

	agent any
	stages{
		stage('SCM Checkout'){
		   git 'https://github.com/Rahul-Dhama/DhamaKiRepository'
		}
		stage('Compile-Package'){
		   def mvnHome =tool name: 'Maven', type: 'maven'
			sh "${mvnHome}/bin/mvn package"
		}
	}		
	
}
