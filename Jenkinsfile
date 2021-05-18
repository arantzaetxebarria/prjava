pipeline {
    agent any
   
    stages {
        stage('Compilar') {
            steps {
                javac Simple.java
            }
        }
        stage('Ejecutar') {
            steps {
                java Simple
            }
        }
    }
}
