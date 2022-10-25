pipeline {
        agent {
        label 'built-in'
            
        }
        stages {
            stage ('stage-1'){
                steps {
                        sh "chmod -R 777 index.html"
                        sh "docker cp index.html e41a8cdf2a34:/usr/local/apache2/htdocs"
                    
                }
            }
        }
}
