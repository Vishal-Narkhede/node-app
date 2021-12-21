node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {

        def customImage = docker.build("vnark01/webapp:01")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
