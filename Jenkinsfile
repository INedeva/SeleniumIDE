pipeline {
    agent any
    stages {
        stage('Install Dependencies') {
            steps {
                bat 'dotnet add package Selenium.WebDriver.ChromeDriver --version *'
            }
        }
        stage('Build') {
            steps {
                bat 'dotnet build'
            } 
        }
        stage('Test') {
            steps {
                bat 'dotnet test'
            } 
        }
    }
}