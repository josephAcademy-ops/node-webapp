pipeline {
	agent {
	    docker {
	        image 'jenkins/jenkins:lts-jdk17'
		args '-u jlacaolacao -p "Acad_student-jlacaolacao'
	    }
	}
        stages {
	    stage('Clone forked repo') {
	        steps {
		   git 'https://github.com/josephAcademy-ops/node-webapp.git'
		}
	    }
	    stage('Building image') {
		steps {
		    script {
			app = docker.build("node-app-image")
		    }
		}
	    }
	}
}
