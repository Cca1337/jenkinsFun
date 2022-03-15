pipeline{
    agent any
    stages{
        stage("Git Clone"){
            steps{
                echo 'Cloning repo'
                git branch: 'master', url: 'https://github.com/Cca1337/HelloWorld-Springboot-App.git'
            }
        }
        stage("Maven test"){
            steps{
                echo 'Running maven test'
                sh 'mvn test'
            }
        }
        stage("Maven Package"){
            steps{
                echo 'Running maven package'
                sh 'mvn package'
            }
        }
        stage("Maven Deploy"){
            steps{
                echo 'Deploying maven war file to production'
            }
        }           
    }
}