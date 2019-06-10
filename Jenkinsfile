standardPipeline {
  standardNode {
    checkoutStage {}

    stage('Update .version') {
    sh "date +%Y%m%d-${env.BUILD_NUMBER} > .version"
    echo "Set version to ${readFile '.version'}"
    }
    dockerBuildStage {}
  }
}