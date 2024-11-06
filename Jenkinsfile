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
                powershell 'C:\\MyScript\\MyScript.ps1'
            }
        }
    }
}