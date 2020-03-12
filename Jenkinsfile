node {

    checkout scm

    docker.withRegistry('https://ip-ftm-v4-team-dev-docker-local.artifactory.swg-devops.com', 'santoshpawaribm') {

        def customImage = docker.build("ip-ftm-v4-team-dev-docker-local.artifactory.swg-devops.com/ddockerwxxebapp","--build-arg DOCKER_REGISTRY=ip-ftm-v4-team-dev-docker-local.artifactory.swg-devops.com","--pull=true Docker_cicd/DockerImage_J2SE_BRM/docker-context .")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
