pipeline {
	agent any
		stages{
			stage("Compile"){
				steps{
					echo "Compiled";
				}
			}
			stage("Junit"){
				steps{
					echo "JUnit";
				}
			}
			stage("Testing"){
				steps{
					echo "Testing";
				}
			}
			stage("Deploy"){
				steps{
					echo "Deploy";
				}
			}
		}
	post {
	    always {
	        echo "Run Always"
	    }
	    success {
	        echo "Only at success"
	    }
	    failure {
	        echo "Only at failed"
	    }
	    unstable {
	        echo "This will run when run is marked as unstable"
	    }
	    changed {
	        echo "When state of pipeline changed for ex :- prev failing now passing"
	    }
  }
}
