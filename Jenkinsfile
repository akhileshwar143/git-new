pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('checkout') {
            steps {
                echo 'Checkout git repo'
                dir('Demo') {
                    // some block
                    git branch: 'main', credentialsId: 'd0153f56-3786-4d3e-8580-4bea9babc0e1', url: 'https://github.com/akhileshwar143/git-new.git'
                
                    sh "ls -lrta"
                }
            }
        }
    }
}

