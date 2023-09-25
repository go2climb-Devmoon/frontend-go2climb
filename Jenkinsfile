pipeline {
    agent any
    tools {
        nodejs "node"
    }
    stages {
        stage('install dependencias') {
            steps {
                bat 'npm install'
            }
        }
        
       stage('build') {
            steps {
                bat 'npm install'
            }
        }

       stage('build app') {
            steps {
                bat 'npm run build'
            }
        }

      stage('deploy') {
            steps {
                bat 'ng serve'
            }
        }
    }
}
