pipeline{
    agent any
    stages {
        stage('Build'){
            steps{
                bat 'npm install'
                script{
                    powershell '''
                        Write-Output "Hello-script-powershell"
                        $date = Get-Date
                        Write-Output "Current date and time : $date"
                    '''
                }
                script{
                    powershell '''c:\\MyScript\\MyScript1.ps1'''
                }
            }
        }
        stage('PowerShell'){
            steps{
                powershell 'C:\\MyScript\\MyScript2.ps1'
            }
        }
    }
}