pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    bat 'echo Starting Hello World Pipeline'
                    bat 'javac Main.java'  // Ensure the filename matches your class name
                }
            }
        }
        stage('Execute Script') {
            steps {
                script {
                    bat 'java Main'  // Run the compiled Java class
                }
            }
        }
    }
}

