node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockersecret') {

        def customImage = docker.build("satcse321/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
