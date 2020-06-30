node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {

        def customImage = docker.build("syedalii/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
