pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                withAWS(region:'us-west-2', credentials:'AKIA5NUDLZF32AYFZ5YE') {
                    s3Upload(file:'index.html', bucket:'build-pipeline-udacity', path:'index.html')
                }
            }
        }
    }
}
