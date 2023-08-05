pipeline
{
agent any
		Stages {
	            stage ('SCM'){
			steps {
			echo "git pull my code step1"			
			echo "git pull my code step2"
			}
			}


		    stage ('Deploy') {	
			steps {
				echo "deploye my code"
				}
				}



		   stage ('Test') {
			steps {
    			   echo "test the code"
			}
			}
		}
}	 


