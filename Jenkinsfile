pipeline {
     agent { label 'master' }
     stages {
         stage('compile') {
             steps {
                    sh 'mvn compile'

             }
         }
         stage('test') {
             steps {
                    sh 'mvn test'
             }
         }
         stage('packege') {
             steps {
                    sh 'mvn packege'
                 
             }
         }
         
     }  
}
