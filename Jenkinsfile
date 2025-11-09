pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo "Pulling code from GitHub..."
                checkout scm
            }
        }

        stage('Compile') {
            steps {
                echo "Compiling Java program..."
                sh 'javac Hello.java'
            }
        }

        stage('Run Program') {
            steps {
                echo "Running Java program..."
                sh 'java Hello'
            }
        }
    }
}
