pipeline {
    agent any
    stages{
        stage('Build new') {
            steps {
                echo 'Building...'
                }
                post {
                    always {
                        jiraSendBuildInfo branch: '', site: 'testing-devops123.atlassian.net'
                        
                    }
                    
                }
            
        }
    }
}
