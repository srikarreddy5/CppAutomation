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
        stage('Build') {
            steps {
                sh 'make'  # Adjust this if you're using CMake
            }
        }
        stage('Test') {
            steps {
                sh './run_tests.sh'  # Change to your actual test script
            }
        }
        stage('Run') {
            steps {
                sh './program.out'  # Run the compiled program
            }
        }
    }
}
