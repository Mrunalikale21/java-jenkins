pipeline {
   agent any
   tools {
       maven 'Maven 3.8.1'   // Use a pre-configured Maven installation
       jdk 'JDK 11'          // Use a pre-configured JDK installation
   }
   stages {
       stage('Build') {
           steps {
               sh 'mvn clean install'
           }
       }
   }
}
