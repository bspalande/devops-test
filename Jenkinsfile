pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
					sh '''
					echo "Archive file creation start....."
					tar -czvf large_txtfiles.tar.gz large_txtfiles1/s1.txt
					echo "Archive file creation end..."
					echo "moving file start....."
					scp -r large_txtfiles1.tar.gz user@bspalande-ae5be8805.mylabserver.com:/home/user/
					echo "moving file end..."
					'''
		    
            }
        }
		
    }
}
