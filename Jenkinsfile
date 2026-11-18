pipeline {
    agent any

    stages {
        stage('Check Java') {
            steps {
                bat 'where.exe javac'
                bat 'javac -version'
                bat 'where.exe java'
                bat 'java -version'
            }
        }

        stage('Compile') {
            steps {
                echo 'Compiling...'
                bat 'javac HelloWorld.java'
            }
        }

        stage('Run') {
            steps {
                echo 'Running...'
                bat 'java HelloWorld'
            }
        }
    }
}