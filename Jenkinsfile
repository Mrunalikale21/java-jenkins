pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    bat 'echo Starting Hello World Pipeline'
                    bat 'javac HelloWorld.java'  // Ensure the filename matches your class name
                }
            }
        }
        stage('Execute Script') {
            steps {
                script {
                    bat 'java HelloWorld'  // Run the compiled Java class
                }
            }
        }
    }
}

