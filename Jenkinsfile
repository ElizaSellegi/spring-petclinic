pipeline {
    agent any 
    stages {
        stage('Compile') {
            steps {
                build 'PetClinic-Compile'
                echo 'PetClinic-Compile built!' 
            }
        }
        stage('Test') {
            steps {
                build 'PetClinic-Test'
                echo 'PetClinic-Test built!' 
            }
        }
        stage('Archive') {
            steps {
                archive '**/target/*.war'
                echo 'PetClinic Archived!' 
            }
        }
    }
}
