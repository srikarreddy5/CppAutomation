pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/srikarreddy5/CppAutomation.git'
            }
        }
        stage('Check Workspace') {
            steps {
                sh 'ls -lah'  # Check if files exist
            }
        }
        stage('Build') {
            steps {
                sh 'make'  # Run make without cd
            }
        }
        stage('Run Program') {
            steps {
                sh './program.out'  # Run the program without cd
            }
        }
    }
}
