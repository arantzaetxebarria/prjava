pipeline {
    agent any
    environment {
        NOMBRE="Arantza"
    }
   
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
        stage('Compilar con parametros') {
            steps {
                sh 'javac Simple.java'
            }
        }
        stage('Ejecutar con parametros') {
            steps {
                sh 'java Simple $(NOMBRE)'
            }
        }
    }
}
