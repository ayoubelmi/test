/*pipeline {
    agent { dockerfile { 
                  filename 'Dockerfile'
                  label 'docker-agent' } 
          }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
                sh 'svn --version'
            }
        }
    }
}
*/





pipeline {
    agent {
        docker { image 'node:7-alpine' 
               label 'docker-agent'
               }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
        stage('other stage') {
            steps {
                sh 'pwd'
            }
        }
        
    }
}
/*
pipeline {
    agent none
    stages {
        stage('Back-end') {
            agent {
                docker { image 'maven:3-alpine' }
            }
            steps {
                sh 'mvn --version'
            }
        }
        stage('Front-end') {
            agent {
                docker { image 'node:7-alpine' }
            }
            steps {
                sh 'node --version'
            }
        }
    }
}

*/
