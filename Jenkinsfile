pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/your-username/CppAutomation.git'
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
