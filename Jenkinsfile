pipeline {
	agent any

	stages {
		stage('build') {
			steps {
		 		sh 'ant -f build.xml -v'
		 		echo 'hii'
			}
		}
	}

	post {
		always {
			archive 'dist/*.jar'
		}
	}
}