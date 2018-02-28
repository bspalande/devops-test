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
    }
}
