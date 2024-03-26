pipeline {
  
    agent any
    
    tools{
        maven "Maven 3.9.6"
    }

    stages {
        stage('Clone') {
            steps {
               git branch: 'develop', url: 'https://github.com/walkertown/ShoppingApp.git'
            }
        }
        stage('Build') {
            steps {
               sh 'mvn clean package'
            }
        }
    }
}
