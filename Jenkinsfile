pipeline {
    agent any
    stages {
        stage ('SCM'){
            steps {
                echo "git pull my code step1"			
                echo "git pull my code step2"
            }
        }

        stage ('Deploy') {	
            steps {
                echo "deploy my code"
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
