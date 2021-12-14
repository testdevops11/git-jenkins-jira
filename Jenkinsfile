pipeline {
    agent any
    stages{
        stage('Build') {
            steps {
                echo 'Building...'
                }
                post {
                    always {
                        jiraSendBuildInfo branch: 'test-1234', site: 'testing-devops123.atlassian.net'
                        
                    }
                    
                }
            
        }
    }
}
