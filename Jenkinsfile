pipeline {
     agent any { label 'master' }
     stages {
         stage('compile') {
             steps {
                 withMaven(maven : 'maven_3_6_0') {
                    sh 'mvn compile'
                 }
             }
         }
         stage('test') {
             steps {
                 withMaven(maven : 'maven_3_6_0') {
                    sh 'mvn test'
                 }
             }
         }
         stage('packege') {
             steps {
                 withMaven(maven : 'maven_3_6_0') {
                    sh 'mvn packege'
                 }
             }
         }
         
     }  
}
