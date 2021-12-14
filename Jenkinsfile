pipeline {
    agent any
    stages{
        stage('Build') {
            steps {
                echo 'Building...'
                }
                post {
                    always {
                        jiraSendBuildInfo site: 'testing-devops123.atlassian.net'
                        
                    }
                    
                }
            
        }
    }
}
