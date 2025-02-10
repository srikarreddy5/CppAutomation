pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                sh 'rm -rf CppAutomation'  
                sh 'git clone https://github.com/srikarreddy5/CppAutomation.git CppAutomation'
            }
        }
        stage('Check Workspace') {
            steps {
                sh 'pwd'      # Check current directory
                sh 'ls -lah'  # List files
            }
        }
        stage('Build') {
            steps {
                sh 'cd CppAutomation && make'  # Now cd is needed
            }
        }
        stage('Run Program') {
            steps {
                sh 'cd CppAutomation && ./program.out'
            }
        }
    }
}
