pipeline {
    agent {
    	label 'freebsd_12_1'
    }
	stages {
		stage('Install Dependencies') {
			steps {
				sh 'pkg install -y gohugo'
			}
		}
		stage('Build') {
			steps {
				 sh 'hugo'	
			}
		}
        stage('Unit Tests') {
			steps {
				sh 'echo "Unit Tests Here"'
			}
		}
		stage('Publish') {
			steps {
				sh 'echo "Publish Here"'
			}
		}
    }
}

