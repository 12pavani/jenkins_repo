pipeline {
    agent any

    parameters {
        string(name: 'COLOR', defaultValue: 'blue', description: 'Choose a color')
    }

    stages {
        stage('Print Color') {
            steps {
                echo "Selected color is: ${params.COLOR}"
                sh "echo COLOR: ${params.COLOR}"
            }
        }

        stage('Build') {
            steps {
                echo "Simulating build process..."
                sh "sleep 2"
            }
        }
    }
}
