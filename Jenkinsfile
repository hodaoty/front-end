pipeline {
    agent any 

    stages {
        stage('build-step') {
            steps {
                echo 'Building the project'
                sh 'npm install'
            }
        }
        stage('test-step') {
            steps {
                echo 'Running tests'
                sh 'npm test'
            }
        }
        stage('package-step') {
            steps {
                echo 'Packaging the project'
                sh 'npm run package'
            }
        }
    }
    post {
        always {
            echo 'This pipeline has completed ...'
        }
    }
}