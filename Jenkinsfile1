pipeline {
    agent any
    stages {
        stage ('skipcheckout') {
            options {
                skipDefaultCheckout()
            }
        }
        stage ('HW') {
            steps{
                echo 'Hello World'
            }
        }
        stage('Build') {
            steps{
                sh 'echo "Build completed."'
            }
        }
    }
    post {
        always {
            echo 'I will always say hello'
        }
    }
}
