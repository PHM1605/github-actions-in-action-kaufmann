# github-actions-in-action-kaufmann

## Self-hosted runner setup

### Download
```sh
$ mkdir actions-runner && cd actions-runner
$ curl -o actions-runner-osx-x64-2.335.1.tar.gz -L https://github.com/actions/runner/releases/download/v2.335.1/actions-runner-osx-x64-2.335.1.tar.gz
$ echo "b2fe57b2ae5b0bc1605f9fc0723c07eedf06167321d3478ce0440f15e5b0a010  actions-runner-osx-x64-2.335.1.tar.gz" | shasum -a 256 -c
$ tar xzf ./actions-runner-osx-x64-2.335.1.tar.gz
```
### Configure
```sh
# Create the runner and start the configuration experience
$ ./config.sh --url https://github.com/PHM1605/github-actions-in-action-kaufmann --token <RUNNER_TOKEN>
# Last step, run it!
$ ./run.sh
```