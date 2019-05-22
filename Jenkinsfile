pipeline {
    agent any 
    stages {
        stage('--Clean--') {
            steps {
               bat 'mvn clean'
            }
        }
        stage('--Test--') { 
            tools{
                jdk 'JAVA_HOME'   
                }
            steps {
                bat 'java -version'
                bat 'mvn test'
            }
        }
        stage('--Package--') { 
           tools{
                jdk 'JAVA_HOME'   
                }
            steps {
                bat 'java -version'
                bat 'mvn package'
            }
        }
    }
}
