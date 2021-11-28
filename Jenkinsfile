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
            }
        }
    }
}
