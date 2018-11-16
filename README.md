# Moto Server

This is a Docker image which allows you to run the moto mock AWS server: https://github.com/spulec/moto#stand-alone-server-mode

## Usage

The basic usage is to pass the service you want to run as a command to the container:

```
docker container run mergermarket/motoserver <service>
```

For example, the EC2 service and using port 6000 (default is 5000):

```
docker container run --rm -p 6000:6000 mergermarket/motoserver ec2 -p 6000
```
