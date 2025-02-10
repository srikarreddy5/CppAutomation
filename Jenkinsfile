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
                sh 'pwd'      # Print current directory
                sh 'ls -lah'  # List files
            }
        }
    }
}
