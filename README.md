DynamoDB tutorial based on the official [AWS documentation](http://docs.aws.amazon.com/amazondynamodb/latest/gettingstartedguide/GettingStarted.Python.html)

## Environment Setup
1. `conda create -n dynamoDB python=3 ipython ipython-notebook boto3`
2. `docker pull tutum/dynamodb` [local instance of dynamodb](https://hub.docker.com/r/tutum/dynamodb/)
3. `docker run -d -p 8000:8000 --name dynamoDB -v /your/path/to/store/db:/data tutum/dynamodb`

To get the ip to use in the `endpoint_url`, run `docker-image ls`.