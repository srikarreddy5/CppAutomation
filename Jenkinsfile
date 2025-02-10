pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/srikarreddy5/CppAutomation.git'
            }
        }
        stage('Build') {
            steps {
                sh 'make'  # No cd needed
            }
        }
        stage('Run Program') {
            steps {
                sh './program.out'  # No cd needed
            }
        }
    }
}
