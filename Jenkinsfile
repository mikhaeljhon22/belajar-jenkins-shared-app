@Library("belajar-jenkins-shared@main") _

import programmerzamannow.jenkins.Output;

pipeline{
    agent any

    stages{
        stage("Hello Groovy"){
            steps{
                script{
                    Output.hello("groovy")
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
    }
}