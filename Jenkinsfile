pipeline {
    agent any

    tools {
        maven 'maven'
    }

    stages {
        stage('Build') {
            steps {
                git branch: 'main', credentialsId: 'jenkinsDamal', url: 'https://github.com/vantaram/santosh1.git'
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
		stage('maven deploy') {
            steps {
                sh 'mvn deploy'
                   }
			            }
		
			}			
	}