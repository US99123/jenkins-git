pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'echo "Hello World 1"'
                bat '''
                    echo "Multiline shell steps works too."
                '''
				bat 'echo "Hello there."'
				
            }
        }
    }
}
