pipeline {
	agent any
	stages {
		stage('BUILD') {
			steps {
				sh '''
					pwd
					sleep 5
					echo This is the fist stage: BUILD
				'''
			}	
		}
		
		stage('TEST') {
			parallel {
			stage('one') {
			steps {
				sh 'pwd'
			}
			stage('two') {
			steps {
				sh 'ls'
			}
			}
			}
		}
		}


		}
		
		stage('DEPLOY') {
			steps {
				sh '''
					pwd
					sleep 5
					echo This is the fist stage: DEPLOY
				'''
			}
		}
	}
}
