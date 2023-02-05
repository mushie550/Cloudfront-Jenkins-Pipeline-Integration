pipeline {
    agent any
    stages {
        stage('deploy') {
            steps {
              
              sh "aws s3 cp index.html s3://demo-cloudfront-s3-bucket0"
            }
        }
    }
}
