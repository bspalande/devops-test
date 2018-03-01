pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
					sh '''
					tar -czvf large_txtfiles.tar.gz large_txtfiles/s1.txt
					echo "This will run only if the run was marked as unstable"
					'''
		    
            }
        }
		stage ('Deploy') {
			steps {
					sh '''
					
					sh 'scp -r large_txtfiles.tar.gz user@bspalande-ae5be8805.mylabserver.com:/home/user/'
					'''
					
					
					}
				}
    }
}
