pipeline {

    agent any

    tools {

        maven 'maven'

    }

    environment {
        TENANT_ID="bf014b4a-f9e8-44bb-9e5d-688eee4115e0"
    }

    stages {
        stage('Check Out from Git') 
        {
            steps {
                git branch: 'prod' , url: 'https://github.com/bkrrajmali/azure-evening-springbootjavapp.git'
            }
        }

        /*
        stage('Maven Validate') 
        {
            steps {
                sh 'mvn validate'
            }
        }

        stage('Maven Compile') 
        {
            steps {
                sh 'mvn compile'
            }
        }
        stage('Maven Test') 
        {
            steps {
                sh 'mvn test'
            }
        }
        stage('Maven Install') 
        {
            steps {
                sh 'mvn install'
            }
        }
        stage(' Trivy Scan')
        {
            steps {
                echo "Trivy Scan Started"
                sh 'trivy fs --format table --output trivy-report.txt --severity HIGH,CRITICAL .'
                echo "Trivy Scan Finished"
            }
        }
        */
    }
    
}