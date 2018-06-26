pipeline {
    agent any
    stages{
        stage("Checkout POint"){
            steps{
                cleanWs()
                // first repository
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: 'Checkout-Dir']], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/KrutikaShah52/Git_checkout_pipeline_jenkins.git']]])
                echo "chaeckout done"
                // run first script
                // load 'subdirectory1/Jenkinsfile'
            }
        }
    }
}


// node {
//     cleanWs()
//     // first repository
//     checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: 'Checkout-Dir']], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/KrutikaShah52/Git_checkout_pipeline_jenkins.git']]])
//     echo "chaeckout done"
//     // run first script
//     // load 'subdirectory1/Jenkinsfile'
// }

