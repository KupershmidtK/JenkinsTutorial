/* Requires the Docker Pipeline plugin */
pipeline {
    agent { label 'host' }
    stages {
        stage('build') {
            steps {
		script {
            	    docker.image('maven:3.9.12-eclipse-temurin-21-alpine').inside {
			sh 'mvn --version'
		    }
		}
            }
        }
    }
}
