
node {
/*
    // Get Artifactory server instance, defined in the Artifactory Plugin administration page.
    def server = Artifactory.server "spdevops"
    // Create an Artifactory Maven instance.
    def rtMaven = Artifactory.newMavenBuild()
    def buildInfo
    
    rtMaven.tool = "maven"
    
    stage('Clone sources') {
        git url: 'https://github.com/sanghoonp3/webapp.git'
    }
    */
    /*
    stage('Artifactory configuration') {
        // Tool name from Jenkins configuration
        rtMaven.tool = "maven"
        // Set Artifactory repositories for dependencies resolution and artifacts deployment.
        rtMaven.deployer releaseRepo:'libs-release-local', snapshotRepo:'libs-snapshot-local', server: server
        rtMaven.resolver releaseRepo:'libs-release', snapshotRepo:'libs-snapshot', server: server
    }

    stage('Maven build') {
        buildInfo = rtMaven.run pom: 'pom.xml', goals: 'clean install'
    }

    stage('Publish build info') {
        server.publishBuildInfo buildInfo
    }
    */
	
 {				//indicate the job is written in Declarative Pipeline
    agent any				//agent specifies where the pipeline will execute. 
    stages {
        stage ("build") {		//an arbitrary stage name
            steps {
                build 'Pipeline_B'	//this is where we specify which job to invoke.
            }
        }
    }
}
	 
