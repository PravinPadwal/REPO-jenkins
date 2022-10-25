pipeline {
        agent {
        label 'built-in'
            
        }
        stages {
            stage ('stage-2'){
                steps {
                 sh "chmod -R 777 index.html"   
                 sh "docker cp index.html 10e42376a542:/usr/local/apache2/htdocs"
                }
            }
        }
}
