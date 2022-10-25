pipeline {
        agent {
        label 'built-in'
            
        }
        stages {
            stage ('stage-1'){
                steps {
                    sh "docker cp index.html a1b6cbbdf112:/usr/local/apache2/htdocs"
                }
            }
        }
}
