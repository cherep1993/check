pipeline {
    agent any
    tools {nodejs "nodeV16"}
    
    stages {
        stage('Install') { 
            steps {
                bat 'npm install' 
            }
        }
        // stage('Test') { 
        //     steps {
        //         bat 'npm test' 
        //     }
        // }
        stage('Build') { 
            steps {
                // bat 'npm run build'
                // bat 'npm install -g serve'
                // bat 'serve -s build -l 3000'
                bat 'npm run deploy'
            }
        }
    }
}