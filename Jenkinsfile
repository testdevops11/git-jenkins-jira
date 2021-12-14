pipeline {
    agent any
    stages{
        stage('Build new project') {
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
