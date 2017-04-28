#!groovy
pipeline{
	agent {label 'mvn-compile'}
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