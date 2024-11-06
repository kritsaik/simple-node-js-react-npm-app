pipeline{
    agent any
    stages {
        stage('Build'){
            steps{
                bat 'npm install'
            }
        }
        stage('PowerShell'){
            steps{
                PowerShell 'C:\\MyScript\\MyScript.ps1'
            }
        }
    }
}