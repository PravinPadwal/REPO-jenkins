pipeline {
        agent {
        label 'built-in'
            
        }
        stages {
            stage ('stage-1'){
                steps {
                    sh "docker cp index.html 84c9d16fd3ef:/usr/local/apache2/htdocs"
                }
            }
        }
}
