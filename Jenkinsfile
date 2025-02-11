pipeline {
    agent any

    }
    stages {

        stage('restore') {
            steps {
                script { // This is Optional buf if i want o run two commands then i need script 
                    sh 'dotnet restore'
                    // sh 'dotnet build' // If i have this i will need the script

                }
            }
        }

        stage('build') {
            steps {
                sh 'dotnet build'
            }
        }

        stage('test') {
            steps {
                sh 'dotnet test'
            }
        }
    }
}
