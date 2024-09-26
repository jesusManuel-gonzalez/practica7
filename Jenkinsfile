pipeline {
    agent any

    stages {
        stage('Clonar') {
            steps {
                git url: 'https://github.com/<nombre del repositorio>.git', credentialsId: '<ID-de-la-credencial>'
            }
        }
        stage('Instalar Dependencias') {
            steps {
                sh 'npm install'
            }
        }
        stage('Ejecutar Pruebas') {
            steps {
                sh 'npm test'
            }
        }
    }
}
