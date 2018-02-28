pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
					sh '''
					
					tar -czvf large_txtfiles.tar.gz large_txtfiles/*.txt
					scp large_txtfiles.tar.gz user@bspalande-ae5be8805.mylabserver.com:/home/user/
					'''
            }
        }
    }
}
