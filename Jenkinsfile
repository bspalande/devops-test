pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
					sh '''
					tar -czvf large_txtfiles.tar.gz large_txtfiles/*.txt
					'''
		    
            }
        }
		stage ('Deploy') {
			steps {
					sh '''
					sudo su - user
					ssh user@bspalande-ae5be8805.mylabserver.com
					'''
					
					
					}
				}
    }
}
