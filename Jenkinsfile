pipeline {
    agent any
    tools{ jdk 'jdk8' }
    stages {
        stage ('Compile Stage') {
            steps {
                withMaven(maven : 'maven3') {
                    bat 'mvn clean compile'
                }
            }
        stage ('Testing Stage') {
            steps {
                withMaven(maven : 'maven3') {
                    bat 'mvn test'
                } }}
        stage ('Install Stage') {
            steps {
                withMaven(maven : 'maven3') {
                    bat 'mvn install'
                } } } }}
