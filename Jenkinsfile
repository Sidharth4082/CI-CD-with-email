pipeline{
    agent any
    
    stages {
        stage ('Code Check') {
            steps {
                echo 'This step will check your code'
            }
            
            
        }
        
        stage ('Build') {
            
            steps {
                
                echo 'This step will make a build for you '
            }
        }
        stage ('Run') {
            
            steps {
                
                echo 'This step will run you code locally'
                
            }
            
        }
        stage ('Deploy') {
            steps {
                echo 'This tep will deploy your build into production'
            }
            
            
        }
    }
    
    post {
        always {
            emailext body: '''Hi Sidharth ''', subject: 'your build status', to: 'sidhu926250@gmail.com'
        }
    }
}
