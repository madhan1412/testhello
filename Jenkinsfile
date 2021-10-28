pipeline {
    agent any

    stages {

        stage ('It will compile the source code') {
        stage ('Compile Stages') {

            steps {
                withMaven(maven : 'maven') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('It will perform unit testing') {
        stage ('Testing Stages') 

            steps {
                withMaven(maven : 'maven') {
                    sh 'mvn test'
                }
            }
        }


        stage ('IT will install to local maven repository which is .m2') {
        stage ('Deployment Stages') {
            steps {
                withMaven(maven : 'maven') {
                    sh 'mvn install'
                }
            }
        }
    }
}
