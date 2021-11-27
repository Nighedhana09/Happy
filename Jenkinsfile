pipeline {
    agent any

    stages {
        
        stage('Build') {
            steps {
                echo 'Building..'
                //sh'npm install'
                sh'ng build'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                sh'cp -r ${/var/lib/jenkins/workspace/Happy-Project}/build/ /usr/share/nginx/html/happy/'
            }
        }
    }
}
// Script //
node {
    stage('Build') {
        echo 'Building....'
    }
    stage('Test') {
        echo 'Building....'
    }
    stage('Deploy') {
        echo 'Deploying....'
    }
}

