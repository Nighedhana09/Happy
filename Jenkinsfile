pipeline {
    agent any

    stages {
      stage('Install') {
      steps { sh 'npm install' }
    
        stage('Build') {
            steps {
                echo 'Building..'
                sh'npm run build'
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
                 sh'rm -rf /var/www/jenkins-angular-app'
                 sh'cp -r ${WORKSPACE}/build/ /var/www/jenkins-angular-app/'
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
