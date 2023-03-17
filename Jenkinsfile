pipeline {
    agent any 
    stages {
        stage ("clone git") {
            steps {
                sh "https://github.com/deshmukhpoonam/game-of-life.git"
                 }
        }
         stage ("clean"){
             steps {
                 sh "mvn clean"
             }
         }
             stage ("mvn install"){
                 steps {
                 sh "mvn install"
                 }
             }
