@Library('libpipelines@master') _

hose {
    EMAIL = 'eos@stratio.com'
    BUILDTOOL = 'make'
    VERSIONING_TYPE = 'stratioVersion-3-3'
    UPSTREAM_VERSION = '2.1.4'
    DEPLOYONPRS = true
    DEVTIMEOUT = 30
    ANCHORE_POLICY = "production"
    GRYPE_TEST = false

    DEV = { config ->
        doDocker(conf:config, dockerfile: 'Dockerfile', image:'cluster-api-provider-aws')
    }
}
