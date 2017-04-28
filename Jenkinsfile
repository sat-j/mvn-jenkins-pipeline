#!groovy
pipeline{
	agent any
	tools { 
        maven 'M3'
        jdk 'JDK'
    }
	stages {
		
		stage('clean'){
			steps{
				sh 'mvn clean'
			}
		}
		
		stage('build'){
			steps{
				sh '''
					mvn package
				'''
			}
		}
	}
	

}