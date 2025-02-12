pipeline {
    agent { label 'agent1' }

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'echo "Starting Hello World Pipeline"'
                    sh 'javac HelloWorld.java'  // Compile Java file
                }
            }
        }
        stage('Execute Script') {
            steps {
                script {
                    sh 'java HelloWorld'  // Run the compiled Java class
                }
            }
        }
    }
}
