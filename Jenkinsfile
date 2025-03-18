pipeline {
    agent any
    stages {
        stage('Checkout') {          
            steps {
                git branch: 'main', url: 'https://github.com/MadhavMadan336/Maven.git'
            }
        }
        stage('Build') {
            steps {
                // Use Maven to build your project
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                // Run tests if applicable
                sh 'mvn test'
            }
        }
    }
}
