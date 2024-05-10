pipeline {
    agent any

    stages {
        stage('Remove Repository') {
            steps {
                // Remove the existing repository directory
                deleteDir()
            }
        }
        stage('Clone Repository') {
            steps {
                // Clone the repository
                git 'https://github.com/SadiqaKhursheed/JenkinsRepo.git'
            }
        }
        stage('Run Code') {
            steps {
                // Run the Python code
                sh 'python jenkinsWork.py'
            }
        }
    }
}
