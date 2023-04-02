pipeline{
    agent any

    stages{
stage('Git Checkout'){
    steps{
        script{
            gitCheckout(
                branch: "main",
                url:"https://github.com/grteja9/Jenkins_Shared_Lib.git"
            )
        }
    }
}

    }
}