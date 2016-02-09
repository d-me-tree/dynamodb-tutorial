Python3 DynamoDB tutorial based on the official [AWS documentation](http://docs.aws.amazon.com/amazondynamodb/latest/gettingstartedguide/GettingStarted.Python.html). I use [this](https://hub.docker.com/r/tutum/dynamodb/) docker image to run a local instance of DynamoDB.

## Environment Setup
1. `conda create -n dynamoDB python=3 ipython ipython-notebook boto3`
2. `docker pull tutum/dynamodb`
3. `docker run -d -p 8000:8000 --name dynamoDB -v /your/path/to/store/db:/data tutum/dynamodb`

## Docker commands
* `docker run dynamoDB`
* `docker stop dynamoDB`
* `docker-image ls` - useful to get the IP to use in `endpoint_url` when creating dynamodb resource.
