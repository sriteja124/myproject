pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Hello World'
		git branch: 'main', url: 'https://github.com/sriteja124/myproject.git'
            }
        }
	stage("Build") {
           steps {
	       sh 'chmod +x ./pro.sh'
               sh './pro.sh'
		  
	   }
	}
			
    }
}
