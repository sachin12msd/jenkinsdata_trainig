pipeline {
    agent any
    stages {
        stage ('SCM'){
            steps {
                echo "git pull my code step1"			
               git 'https://github.com/sachin12msd/simple-java-maven-app.git'
            }
        }

        stage ('Build) {	
            steps {
		sh 'mvn clean package'
            }
        }

        stage ('Test') {
            steps {
                echo "test the code"
            }
        }
    

	  stage ('Prod') {
            steps {
                echo "deploy in prod"
		}
		}

}
}