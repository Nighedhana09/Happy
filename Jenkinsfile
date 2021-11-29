pipeline {
     agent any
     stages {
        stage("Build") {
            steps {
                sh "npm install"
                sh "npm run ng --build"
            }
        }
        stage("Deploy") {
            steps {
             echo  "deployed"
             sh "sudo rsync -a /var/lib/jenkins/workspace/Happy-Project /var/www/angular-cicd"
            }
        }
    }
}
