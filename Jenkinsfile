node {

    checkout scm

    docker.withRegistry('https://ip-ftm-v4-team-dev-docker-local.artifactory.swg-devops.com', 'santoshpawaribm') {

        def customImage = docker.build("ip-ftm-v4-team-dev-docker-local.artifactory.swg-devops.com/ddockerwxxebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
