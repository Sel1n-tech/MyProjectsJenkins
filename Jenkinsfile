// Jenkinsfile2

pipeline {
    agent any
    stages {
        stage('Prepare') {
            steps {
                echo 'Preparing workspace...'
                sh 'mkdir -p build'
                sh 'mkdir -p log'
                sh 'mkdir -p temp'
                echo 'Directories created'
            }
        }
        stage('Build') {
            steps {
                echo 'Building application...'
                sh 'echo "Build version: 1.0.0" > build/version.txt'
                sh 'date >> build/version.txt'
                echo 'Build completed'
             }
        }
         stage('Verify') {
            steps {
                echo 'Verifying build...'
                sh 'cat build/version.txt'
                sh 'ls -la build/'
                echo 'Verification completed'
        }
        }

        stage('System Info') {
            steps {
                echo 'System Information WaTaFAAA'
                echo 'Collecting 3A GAMES'
                echo "Build Number: ${BUILD_NUMBER}"
                echo "Job Name: ${JOB_NAME}"
                echo 'System info collection finished'
                sh 'whoami'
                sh 'df -h .'
                sh 'uname -a'
            }
        }
    }
}
