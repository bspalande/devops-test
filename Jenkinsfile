pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
		tar -czvf /home/user/devops-test/large_txtfiles.tar.gz /home/user/devops-test/large_txtfiles/'*.txt'
		scp /home/user/devops-test/large_txtfiles.tar.gz user@bspalande-ae5be8805.mylabserver.com:/home/user/
		ssh user@bspalande-ae5be8805.mylabserver.com
		tar -xvzf /home/user/large_txtfiles.tar.gz -C /
            }
        }
    }
}
