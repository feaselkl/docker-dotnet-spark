# .NET for Spark on a Docker Container

This is a riff on [Ed Elliott's example project](https://github.com/GoEddie/docker-dotnet-spark) for running Apache Spark and .NET Core in a Docker container.

Ed has a pair of outstanding articles on the topic.  This project stems from [a post Ed wrote](https://the.agilesql.club/2019/07/spark-and-dotnet-in-a-single-docker-container/), and I also highly recommend [his Simple-Talk article](https://www.red-gate.com/simple-talk/dotnet/net-development/apache-spark-for-net-developers/).

## Requirements

You must have Docker configured to run Linux containers.

## Instructions

After downloading this, navigate to the folder and run the following to build the container and execute it:

```
docker build -t dotnet-spark .
docker run -it dotnet-spark bash
cd /root
./run_spark_dotnet_demo
```

## Additional Notes

The `run_spark_dotnet_demo` script pulls an F# project from another repo of mine, at https://github.com/feaselkl/Getting-Started-With-Apache-Spark.
