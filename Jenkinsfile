@Library('my-shared-library') _
customWorkspace='/opt/Workspace/grteja_java_app/'
pipeline{
    agent any
      stages{
        stage('Git Checkout'){
            steps{
                script{
                        dir('customWorkspace')
                        gitCheckout(
                        branch: "main",
                        url:"https://github.com/grteja9/Jenkins_Shared_Lib.git"
            )
        }
    }
}
        stage('Unit Test Maven'){
            steps{
                script{
                    dir('customWorkspace')
                        mvnTest()
        }
    }
}

    }
}