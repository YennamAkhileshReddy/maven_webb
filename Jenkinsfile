pipeline {
     agent { label 'master' }
     stages {
         stage('compile') {
             steps {
                 withMaven(maven : 'mvn3.6.0') {
                    sh 'mvn compile'
                 }
             }
         }
         stage('test') {
             steps {
                 withMaven(maven : 'mvn3.6.0') {
                    sh 'mvn test'
                 }
             }
         }
         stage('packege') {
             steps {
                 withMaven(maven : 'mvn3.6.0') {
                    sh 'mvn packege'
                 }
             }
         }
         
     }  
}
