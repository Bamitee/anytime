# pipeline{
    
    agent any

    stages{

        stage("build") {

            steps{
                echo 'building my application...'

            }
        }        

        stage("test") {
            steps {
                git 'https://github.com/Bamitee/anytime/Kubernetted-Demo .git'

            }

        }

        stage("deploy") {
            steps {
                echo 'deploying my application...'
            }    
        }                  
    }    
}    
# Groovyscript
