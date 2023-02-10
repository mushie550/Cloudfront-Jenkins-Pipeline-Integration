pipeline {
    agent any
    stages {
        stage('deploy') {
            steps {            
              sh "aws s3 sync . s3://demo-cloudfront-s3-bucket0"
              sh "aws cloudfront create-invalidation --distribution-id E3SJLO9P6GD5DO --paths "/*""
            }
        }
    }
}
