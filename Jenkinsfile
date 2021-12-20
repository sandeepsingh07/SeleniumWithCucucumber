pipeline {
  agent any
  tools{
    maven 'maven'
    jdk 'java'
}
  stages {
    
       stage('Maven') {
          steps {
            echo 'Running from Jenkins file'
            sh(script: 'mvn compile', label: 'maven')
          }
        }

        stage('Cucumber') {
          steps {
            cucumber '**/*.json'
          }
        }

      }
    }

