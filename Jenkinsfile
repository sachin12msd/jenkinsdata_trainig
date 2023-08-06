pipeline {
    agent any
    stages {
        stage('SCM') {
            steps {
                echo "git pull my code step1"			
                git 'https://github.com/sachin12msd/simple-java-maven-app.git'
            }
        }

        stage('Build') {
            steps {
                sh 'sudo mvn clean package'
            }
        }

        stage('Deploye') {
            steps {
                sh 'sudo java -jar target/*.jar'
            }
        }
    
        stage('Prod') {
            steps {
                echo "deploy in prod"
            }
        }
    }
}
