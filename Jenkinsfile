pipeline {
    agent any
   
    stages {
        stage('Compilar') {
            steps {
                javac Param.java
            }
        }
        stage('Ejecutar') {
            steps {
                java Param
            }
        }
    }
}
