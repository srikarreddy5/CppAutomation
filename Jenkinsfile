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
                sh '''
                make
                '''
            }
        }
        stage('Run Program') {
            steps {
                sh '''
                ./program.out
                '''
            }
        }
    }
}
