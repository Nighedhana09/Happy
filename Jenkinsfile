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
              sh "sudo cp -r ${/var/lib/jenkins/workspace/Happy-Project}/build/  /usr/share/nginx/html"
            }
        }
    }
}
