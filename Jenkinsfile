pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'dotnet build'
            } 
        }
        stage('Install Dependencies') {
            steps {
                bat 'dotnet add package Selenium.WebDriver.ChromeDriver --version *'
            }
        }
        stage('Test') {
            steps {
                bat 'dotnet test'
            } 
        }
    }
}