pipeline {
    agent any
    stages {
        stage('SCM') {
            steps {
                echo "git pull my code step1"			
                git 'https://github.com/sachin12msd/simple-java-maven.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Deploye') {
            steps {
                sh 'java -jar target/*.jar'
            }
        }
    
        stage('Prod') {
            steps {
                echo "deploy in production"
            }
        }
    }
}
