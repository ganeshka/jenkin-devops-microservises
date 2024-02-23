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
	}

	 success {
        mail(from: "gnkangne@gmail.com",
                to: "gnkangane@gmail.com",
                subject: "That build passed.",
                body: "Nothing to see here")
    }

    failure {
        mail(from: "gnkangne@gmail.com",
                to: "gnkangane@gmail.com",
                subject: "That build failed!",
                body: "Nothing to see here")
    }
	
}