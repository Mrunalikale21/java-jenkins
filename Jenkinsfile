pipeline {
    agent { label 'agent1' }

    stages {
        stage('Build') {
            steps {
                script {
                    bat 'echo Starting Hello World Pipeline'
                    bat 'dir'  // Debugging: List files in the workspace
                    bat 'javac HelloWorld.java'  // Ensure HelloWorld.java is present
                }
            }
        }

        stage('Execute Script') {
            steps {
                script {
                    bat 'java -cp . HelloWorld'  // Ensure the classpath is set correctly
                }
            }
        }
    }
}

