pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the repository
                git 'https://github.com/dirkagithubs/my_project_jinkens.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                // Build the Docker image using the Dockerfile in the repository
                script {
                    docker.build("my-web-app")
                }
            }
        }

        stage('Run Docker Container') {
            steps {
                // Run the Docker container
                script {
                    docker.run("my-web-app")
                }
            }
        }
    }
}
