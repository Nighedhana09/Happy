pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                "npm install"
                "npm run build"
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
                 "rm -rf /var/www/jenkins-angular-app"
                 "cp -r ${WORKSPACE}/build/ /var/www/jenkins-angular-app/"
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
