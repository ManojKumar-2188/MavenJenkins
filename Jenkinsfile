pipeline {
    agent any

    stages {
        stage("Git clone") {
            steps {
               git branch: 'main', url: 'https://github.com/ManojKumar-2188/MavenJenkins.git'
            }
        }
        
        stage("Maven Test") {
            steps {
               sh 'mvn test'
            }
        }
        
        stage("Maven Build") {
            steps {
               sh 'mvn package'
            }
        }
        
    }
}
