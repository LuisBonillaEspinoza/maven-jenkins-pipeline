pipeline {
    agent any
    tools {
	maven "Maven 3.8.7"
    }

    stages {
        stage('Build Artifact') {
            steps {
                sh "mv clean package -DskipTests=true"
		archive 'target/*.jar'
            }
        }
    }
}