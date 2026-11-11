pipeline {
    agent any
    stages {
        stage('Verify') {
            steps {
                sh label: 'Run tests', script: 'npm test'
                sh(returnStatus: true, label: 'Lint', script: 'npm run build')
            }
        }
    }
}
