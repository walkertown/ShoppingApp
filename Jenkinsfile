pipeline {
  
    agent {
        label 'Java-Node'
    }
    
    tools{
        maven "Maven-3.9.6"
    }

    stages {
        stage('Clone') {
            steps {
               git 'https://github.com/walkertown/ShoppingApp.git'
            }
        }
        stage('Build') {
            steps {
               sh 'mvn clean package'
            }
        }
    }
}
