pipeline {
    agent any

    stages {
        stage('SCM Checkout') {
            steps {
               git branch: 'main', url: 'https://github.com/Prajwalatkare1/Demo-Repo.git'
                // git url: 'https://github.com/your-repo.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the code...'
                // sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                // sh './deploy.sh'
            }
        }
    }
}
