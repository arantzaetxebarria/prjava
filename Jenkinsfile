pipeline {
    agent any
    environment  {
        NOMBRE = "Arantza"
        MAQUINA = """${sh(
        returnStdout: true,
        script: 'uname -n'
        )
        }"""
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
                sh 'javac Param.java'
            }
        }
        stage('Ejecutar con parametros') {
            steps {
                sh 'java Param ${NOMBRE}'
            }
        }
        /*stage('nombreMaquina'){
            steps{
            echo "Y aquí visualizeo el nombre de la maquina "
            sh 'javac Maquina.java'
            sh 'java Maquina ${MAQUINA}'
            }
       }*/
    }
}
