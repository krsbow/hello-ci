pipeline {
    agent any
    tools { nodejs 'node20' }
    stages {
        stage('Install') { steps { sh 'rm -rf node_modules package-lock.json' sh 'npm install' } }
        stage('Test') { steps { sh 'npm test' } }
    }
}
