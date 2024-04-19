pipeline {
    agent any
    
    tools{
        jdk 'jdk17'
        maven 'maven3'
    }

    stages {
        stage('Git Checkout') {
            steps {
                git branch: 'feature-01', url: 'https://github.com/prashantritgit/Petclinic.git'
            }
        }
        
        
        stage('Compile') {
            steps {
                sh "mvn clean compile"
            }
        }
        
        stage('Compile Package') {
            steps {
                sh "mvn clean package"
            }
        }
        
        
        
    }
}
