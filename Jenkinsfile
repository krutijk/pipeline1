pipeline {
    agent any
    stages {
        stage('One') {
                steps {
                        echo 'Hi, this is Kruti'
			
                }
        }
	    stage('Two'){
		    
		steps {
			input('Do you want to proceed?')
        }
	    }
        stage('Three') {
                when {
                        not {
                                branch "master"
                        }
                }
                steps {
			echo "Hello"
                        }
        }
        stage('Four') {
                parallel {
                        stage('Four A') {
                                steps{
                                        echo "Four A running"
                                }
                        }
                        stage('Four B') {
				steps {
					echo 'Four B running'
				}
                               
			}  }
        }
    }
}
