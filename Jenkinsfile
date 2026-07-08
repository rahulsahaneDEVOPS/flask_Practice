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

        stage('Deploy') {
            steps {
                sh '''
                echo "Starting deployment..."

                mkdir -p deployment

                cp app.py deployment/
                cp requirements.txt deployment/
                cp -r templates deployment/

                echo "Application deployed to staging directory."

                ls -l deployment
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