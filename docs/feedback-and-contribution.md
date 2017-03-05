# Feedback and Contribution

TODO: Review

The *Docker Flow: Proxy* project welcomes, and depends, on contributions from developers and users in the open source community. Contributions can be made in a number of ways, a few examples are:

* Code patches or new features via pull requests
* Documentation improvements
* Bug reports and patch reviews

## Reporting an Issue

Feel fee to [create a new issue](https://github.com/vfarcic/docker-flow-cron/issues). Include as much detail as you can.

If an issue is a bug, please provide steps to reproduce it.

If an issue is a request for a new feature, please specify the use-case behind it.

## Discussion

Please join the [DevOps20](http://slack.devops20toolkit.com/) Slack channel if you'd like to discuss the project or have a problem you'd like us to solve.

## Contributing To The Project

I encourage you to contribute to the *Docker Flow Cron* project.

The project is developed using *Test Driven Development* and *Continuous Deployment* process. Test are divided into unit and integration tests. Every code file has an equivalent with tests (e.g. `reconfigure.go` and `reconfigure_test.go`). Ideally, I expect you to write a test that defines that should be developed, run all the unit tests and confirm that the test fails, write just enough code to make the test pass, repeat. If you are new to testing, feel free to create a pull request indicating that tests are missing and I'll help you out.

Once you are finish implementing a new feature or fixing a bug, run the *Complete Cycle*. You'll find the instructions below.

### Repository

Fork [docker-flow-cron](https://github.com/vfarcic/docker-flow-cron).

TODO: Remove

```bash
go build -v -o docker-flow-cron && ./docker-flow-cron
```

### Unit Testing

```bash
docker-compose -f docker-compose-test.yml run --rm unit
```

### Building

```bash
docker-compose -f docker-compose-test.yml run --rm unit

docker build -t $DOCKER_HUB_USER/docker-flow-cron .
```

### The Complete Cycle (Unit, Build, Staging)

TODO

### Pull Request

TODO

Once the feature is done, create a pull request.