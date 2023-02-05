pipeline {
    agent any
    stages {
        stage('deploy') {
            steps {
              
              sh "aws s3 sync index.html s3://demo-cloudfront-s3-bucket0"
            }
        }
    }
}
