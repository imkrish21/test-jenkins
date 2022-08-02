node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'Docker') {

        def customImage = docker.build("Gokul/goki")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
