pipeline {
    agent any
    tools {
        nodejs "node"
    }
    stages {
        stage('Install Dependencias') {
            steps {
                // Instala las dependencias del proyecto
                bat 'npm install'
            }
        }
        
        stage('Build') {
            steps {
                // Realiza una construcción de producción de la aplicación Angular
                bat 'npm run build'
            }
        }

        stage('Start App') {
            steps {
                // Inicia la aplicación Angular localmente
                bat 'npm start'
            }
        }
    }
}
