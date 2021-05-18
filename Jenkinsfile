pipeline {
    agent any
   
    stages {
        stage('Compilar') {
            steps {
                sh 'javac Simple.java'
            }
        }
        stage('Ejecutar') {
            steps {
                sh 'java Simple'
            }
        }
    }
}
