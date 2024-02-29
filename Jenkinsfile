pipeline {
    agent any
    stages {
        stage('deploy') {
            steps {            
              sh "aws s3 sync . s3://demo-task-jenkins"
              sh "aws cloudfront create-invalidation --distribution-id E17769MG412GA2 --paths '/*'"
            }
        }
    }
}
