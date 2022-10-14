pipeline {
 agent {
        label {
            label "built-in"
            customWorkspace "/mnt/ws-3"
        }
    }
    stages {
        stage('installing apache')
        {
            steps
            {
                sh "yum install httpd -y"
            }
        }
        stage ('server start')
        {
            steps
            {
                sh "service httpd start"
            }
        }
        stage ('deploying index.html')
        {
            steps
            {
                sh "cp -r /root/index.html /var/www/html/"
                sh "chmod -R 777 /var/www/html"
            }
        }
    }
}
