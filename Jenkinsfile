pipeline{
    agent any

    tools{
        maven 'maven3.9'
    }
    stages{
        stage("Checkout Code"){
            steps{
                git branch: 'main', url: 'https://github.com/padmanava9490/java-web-app.git'
            }
        }
        stage("Build Code"){
            steps{
                sh 'mvn clean package'
            }
        }
    }
}