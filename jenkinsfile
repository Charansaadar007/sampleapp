pipeline {
    agent any

    stages {
        stage('fetch code') {
            steps {
               git branch: 'main', url: 'https://github.com/Charansaadar007/sample-java.git'
            }
        }
        stage('install apache') { // Corrected stage name
            steps {
               sh 'sudo apt install apache2 -y'
            }
        }
        stage('deploy app') {
            steps {
               sh 'sudo cp -R * /var/www/html/'
            }
        }
    }
}
