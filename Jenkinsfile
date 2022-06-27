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
        stage('Deploy') { 
            steps {
                // bat 'npm run build'
                // bat 'npm install -g serve'
                // bat 'serve -s build -l 3000'
                bat 'git config --global user.email "alla.rakhimova103@gmail.com"'
                bat 'git config --global user.name "Alla Rakhimova"'
                bat 'npm run deploy'
            }
        }
    }
}