pipeline {
     agent { label 'master' }
     stages {
         stage('compile') {
             steps {
                 withMaven(maven : 'maven_3.6.0') {
                    sh 'mvn compile'
                 }
             }
         }
         stage('test') {
             steps {
                 withMaven(maven : 'maven_3.6.0') {
                    sh 'mvn test'
                 }
             }
         }
         stage('packege') {
             steps {
                 withMaven(maven : 'maven_3.6.0') {
                    sh 'mvn packege'
                 }
             }
         }
         
     }  
}
