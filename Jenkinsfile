node{
    stage('Git Checkout'){
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/kvishe/mavenwar.git']]])
    }
    stage('Build'){
        sh 'mvn clean package'
    }
}
