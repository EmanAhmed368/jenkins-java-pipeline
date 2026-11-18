
pipeline {
    agent any

    stages {
        stage('Check Java') {
            steps {
                bat '"C:\\Program Files\\Eclipse Adoptium\\jdk-25.0.5.8-hotspot\\bin\\java.exe" -version'
            }
        }

        stage('Compile') {
            steps {
                echo 'Compiling...'
                bat '"C:\\Program Files\\Eclipse Adoptium\\jdk-25.0.5.8-hotspot\\bin\\javac.exe" HelloWorld.java'
            }
        }

        stage('Run') {
            steps {
                echo 'Running...'
                bat '"C:\\Program Files\\Eclipse Adoptium\\jdk-25.0.5.8-hotspot\\bin\\java.exe" HelloWorld'
            }
        }
    }
}
