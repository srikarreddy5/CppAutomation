pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                sh 'git clone https://github.com/srikarreddy5/CppAutomation.git'
            }
        }
        stage('Build') {
            steps {
                sh '''
                cd CppAutomation
                make
                '''
            }
        }
        stage('Run Program') {
            steps {
                sh '''
                cd CppAutomation
                ./program.out
                '''
            }
        }
    }
}
