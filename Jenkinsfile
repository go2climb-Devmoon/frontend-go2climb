pipeline {
    agent any
    tools {
        nodejs "node" // Asegúrate de que Node.js esté configurado como una herramienta global en Jenkins
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
                bat 'ng build'
            }
        }

        stage('Deploy') {
            steps {
                // Inicia el servidor de desarrollo local con ng serve
                bat 'ng serve --open'
            }
        }
    }
}
