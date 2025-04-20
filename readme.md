Jenkins pipeline uses groovy scripting language, framed out of JAVA
2 types
    scripted(old, all the code inside node block) & declarative(new, all the code inside pipeline block)

I can control the execution of stages(where and when and how) but not the steps 

DECLARATIVE

pipeline {
    agent any(which is free it will execute there, labels give agent name under labels )
    stages {
        stage('Build') {
            steps {
                //
            }
        }
        stage('Test') {
            steps {
                //
            }
        }
        stage('Deploy') {
            steps {
                //
            }
        }
    }
}

SCRIPTED

node {
    stage('Build') {
        //
    }
    stage('Test') {
        //
    }
    stage('Deploy') {
        //
    }
}

PIPELINE SYNTAX

you can edit configurations there 

blue ocean plugin verygood 

of that particular v/sn jenkins file

