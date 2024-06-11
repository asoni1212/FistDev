pipeline {
  agent any

 tools{nodejs 'nodejs'}
stages {
        stage('Build') {
            steps {
                sh 'npm install --legacy-peer-deps'
                sh 'npm install -g less'
                sh 'npm install --save-dev ajv@^7'
                sh 'npm run build'
            }
        }
        stage('Deploy') {
            steps {
              echo "success"
            }
        }
    }
}
