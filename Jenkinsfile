@Library("belajar-jenkins-shared@main") _

import programmerzamannow.jenkins.Output;

pipeline{
    agent any
     tools {
        maven 'maven3'
    }

    stages{
        stage("Hello Groovy"){
            steps{
                script{
                    Output.hello(this,"groovy")
                }
            }
        }
        stage("Hello World"){
            steps{
                script{
                    hello.world()
                }
            }
        }
        stage("Maven Build"){
            steps{
                script{
                    maven(["clean","compile","test"])
                }
            }
        }
        stage("Global Variable"){
            steps{
                script{
                    echo(author())
                    echo(author.name())
                    echo(author.channel())
                }
            }
        }
    }
}