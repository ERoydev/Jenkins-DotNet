pipeline {
    agent any

    
    stages {

        stage('restore') {
            steps {
                script { // This is Optional buf if i want o run two commands then i need script 
                    powershell 'dotnet restore'
                    // sh 'dotnet build' // If i have this i will need the script

                }
            }
        }

        stage('build') {
            steps {
                powershell 'dotnet build'
            }
        }

        stage('test') {
            steps {
                powershell 'dotnet test'
            }
        }
    }
}
