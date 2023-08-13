pipeline {
    agent any

    tools {
        maven 'maven'
    }

    stages {
        stage('Build') {
            steps {
                git branch: 'main', credentialsId: 'jenkinsDamal', url: 'https://github.com/ksrepo9/ks.git'
                   }
			            }
		stage('maven clean') {
            steps {
                sh 'mvn clean'
                   }
			            }
		stage('maven test') {
            steps {
                sh 'mvn test'
                   }
			            }
		stage('mave compile') {
            steps {
                sh 'mvn compile'
                   }
			            }
		stage('maven package') {
            steps {
                sh 'mvn package'
                   }
			            }
		
			}			
	}
	
