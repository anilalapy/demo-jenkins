pipeline {
  agent any
  
  stages {
    
    stage('Checkout') {
      checkout([$class: 'GitSCM',
                branches: [[name: '*/dev']],
                doGenerateSubmoduleConfigurations: false,
                extensions: [[$class: 'CloneOption', noTags: true, reference: '', shallow: true]],
                submoduleCfg: [],
                userRemoteConfigs: [[url: 'https://github.com/anilalapy/demo-jenkins.git']]
                ]);
    }
  
    stage("Build") {
      steps {
        echo "Starting the Build"
      }
    }
    
    stage("Test") {
      steps {
        echo "Starting the Test"
      }
    }
    
    stage("Deploy") {
      steps {
        echo "Starting the Deploy"
      }
    }
  
  }
}
