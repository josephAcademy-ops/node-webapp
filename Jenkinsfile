pipeline {
	agent any

        stages {
	    stage('Clone git') {
	        steps {
		   git 'https://github.com/eMahtab/node-express-hello-world'
		}
	    }
	    stage('Build') {
		steps {
		   git 'https://github.com/eMahtab/node-express-hello-world'
		   sh 'cd node-express-hello-world'
		}
	    }
	    stage('Install npm') {
	    	steps {
		   sh 'npm install'
		}
	    }
	    stage('Start npm') {
	       steps {
		   sh 'npm start'
	       }
	    }
	}
}
