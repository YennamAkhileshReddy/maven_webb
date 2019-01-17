pipeline {
     agent any
     stages {
         stage('compile') {
             steps {
                 withMaven(maven : 'maven_3_6_0') {
                    sh 'mvn clean compile'
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
