pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
		archive 'large_txtfiles/*.txt'
		    bash '''#!/bin/bash
                 echo "hello world" 
         		'''
            }
        }
    }
}
