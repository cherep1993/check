pipeline {
    agent any
    tools {nodejs "nodeV16"}
    
    stages {
        stage('Install') { 
            steps {
                sh 'npm install' 
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
                sh 'git config --global user.email "alla.rakhimova103@gmail.com"'
                sh 'git config --global user.name "Alla Rakhimova"'
                sh 'npm run deploy'
            }
        }
    }
}
