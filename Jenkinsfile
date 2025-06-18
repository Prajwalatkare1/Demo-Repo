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

        stage('Package the Code ') {
            steps {
               withMaven(globalMavenSettingsConfig: '', jdk: '', maven: 'Maven', mavenSettingsConfig: '', traceability: true) {
    // some block
}
                echo 'Packaging the code...'
                 sh 'mvn package'
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
