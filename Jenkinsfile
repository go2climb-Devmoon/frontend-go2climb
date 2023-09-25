pipeline {
    agent any
    tools {
        nodejs "node"
    }
    stages {
        stage('Install Dependencias') {
            steps {
                bat 'npm install'
            }
        }
        
       stage('Build') {
            steps {
                bat 'npm install'
            }
        }

       stage('Build App') {
          steps {
              bat 'ng build'
          }
      }

      stage('Deploy') {
            steps {
                bat 'ng serve'
            }
        }
    }
}
