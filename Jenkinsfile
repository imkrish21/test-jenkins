node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhub') {

        def customImage = docker.build("21killerkong/test-jenkins")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
