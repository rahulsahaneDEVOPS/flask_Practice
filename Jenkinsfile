pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                echo 'Repository cloned successfully'
            }
        }

        stage('Setup Python Environment') {
            steps {
                sh '''
                python3 -m venv venv
                . venv/bin/activate
                pip install --upgrade pip
                pip install -r requirements.txt
                '''
            }
        }

        stage('Run Tests') {
            steps {
                sh '''
                export MONGO_URI="mongodb://localhost:27017/studentdb"
                export SECRET_KEY="rahul123"

                . venv/bin/activate
                pytest -v
                '''
            }
        }

    }

    post {
        always {
            echo 'Pipeline execution completed.'
        }
        success {
            echo 'Build Successful!'
        }
        failure {
            echo 'Build Failed!'
        }
    }
}
