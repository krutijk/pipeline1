pipeline {
    agent any 
        stages {
            stage('One') {
                steps {
                    echo 'Hi! This is Kruti.'
                }
            }
            stage('Two') {
                steps {
                    input('Do you want to proceed?')
                }
            }
            stage('Three') {
		steps {
                	echo 'Hello World!'
		}
            }
            stage('Four') {
                parallel {
                    stage('Four A') {
                        steps {
                            echo 'Four A running.'
                        }
                    }
                    stage('Four B') {
                        steps {
                            echo 'Four B running.'
                        }
                    }
                }
            }
        }
}
