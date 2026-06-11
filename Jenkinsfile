pipeline {
    agent any

    stages{
        stage("Restore dependencies"){
            steps {
                bat "dotnet restore"
            }
        }
        stage("Build"){
            steps{
                bat "dotnet build"
            }
        }
        stage("Run Selenium tests"){
            steps{
                bat "dotnet test"
            }
        }
    }
}