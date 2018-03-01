pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
					sh '''
					echo "Archive file creation start..."
					tar -czvf large_txtfiles.tar.gz large_txtfiles/s1.txt
					echo "Archive file creation end..."
					scp -r large_txtfiles.tar.gz user@bspalande-ae5be8805.mylabserver.com:/home/user/
					'''
		    
            }
        }
		
    }
}
