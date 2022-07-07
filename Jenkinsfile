pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Hello World'
		checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/sriteja124/myproject.git']]])
            }
        }
	stage("Build") {
           steps {
	       sh 'chmod 777 ./pro.sh'
               sh './pro.sh'
		  
	   }
	}
			
    }
}
