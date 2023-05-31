/* Requires the Docker Pipeline plugin */
pipeline {
    agent { docker { image 'node:18.16.0-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'echo "Hello World"'
		sh '''
			echo "Multiline shell script works too"
			ls -lah
		'''
            }
        }
    }
}
