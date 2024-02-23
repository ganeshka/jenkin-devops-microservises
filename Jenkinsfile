pipeline {
//	agent any
agent {
	docker {
		image 'maven:3.9.6'
	}
}
	stages{
		stage('build'){
			steps{
				--sh "mvn --version"
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
	}
}