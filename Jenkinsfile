pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                withMaven(maven : `Maven`)
				sh 'mvn clean compile'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
            
        }
    }
}
