@Library('jenkins-shared-lib')_

stage('SCM CheckOut') {
    printBuildinfo {
        name = "Jenkins Shared Library ! "
    }
} stage('Disable Load balancer') {
    disableBalancerUtils()
} stage('Deploy') {
    deploy()
} stage('Enable Load balancer') {
    enableBalancerUtils()
} stage('Check Status') {
    checkStatus()
}
