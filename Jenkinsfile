pipeline {
    agent any

    tools {
        maven 'Maven' // Make sure 'Maven' is configured under Global Tool Configuration
    }

    stages {
        stage('SCM Checkout') {
            steps {
                echo 'Hello, we started the SCM-Checkout Process'
                git url: 'https://github.com/Prajwalatkare1/maven-project.git'
                echo 'Hello, we ended the SCM-Checkout Process'
            }
        }

        stage('Test the Code') {
            steps {
                echo 'Hello, we started the Code Compile Process'
                sh 'mvn package'
                echo 'Hello, we ended the Compile Process'
            }
        }
    }
}
