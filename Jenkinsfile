pipeline {
	agent any
	stages{
		stage('build'){
			steps{
		echo "Build"			
	}
		}

		stage('test'){
			steps{
		echo "Test"
		
	}
		}

		stage('integration test'){
			steps{
		echo "integration Test3"
		
	}
		}
	}
	post {
		always{
			echo 'I am run always'
		}
		success {
			echo 'I run when you are successfull'
		}
		failure {
			echo 'I run when you fail'
		}
  email 
	{
		to='gnkangne@gmail.com'
	}
	}
	
}