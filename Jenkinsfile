podTemplate {
    node('jenkins-slave') {
        environment {
            dockerhub = credentials('dockerhub_or')
        }
            stage('Build') { 
                        sh 'sudo docker build . -t catalog'
                        sh 'sudo docker run -p 5000:5000 --name catalog catalog &'
                    
                
            
        }
    }
}
