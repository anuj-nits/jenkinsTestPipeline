#!/usr/bin/env groovy
import hudson.model.*
import hudson.EnvVars
import java.net.URL

node{
    stage('Git Checkout'){
        git 'https://github.com/edureka-git/DevOpsClassCodes.git'
    }
    stage('Compile App'){
            withMaven(maven:'Maven 3.6.1'){
            sh 'mvn compile'
        }
    }
    stage('Package App'){
            withMaven(maven:'Maven 3.6.1'){
            sh 'mvn package'
        }
    }
}
