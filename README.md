# docker-android
[![Apache 2.0 License](https://img.shields.io/badge/license-Apache%202.0-blue.svg?style=flat)](http://www.apache.org/licenses/LICENSE-2.0.html)

Docker image for Android builds.

## Base Image

It use CentOS 7 as default base image. But you have another choice base on Ubuntu 14.04. [ubuntu/Dockerfile](ubuntu/Dockerfile).

## What's Included

- Oracle Java 8
- Android SDK
 - Build Tools 25.0.3 & 26.0.3 & 27.0.3
 - Platform SDK 25 & 26 & 27
- Pre-installed Gradle version 4.1

## Usage

You can pull the image form DaoCloud's image repository by using `docker pull` or [`dao pull`](https://dashboard.daocloud.io/mirror).

```sh
docker pull daocloud.io/nicokishi/docker-android:<lastest-verion>
dao pull daocloud.io/nicokishi/docker-android:<lastest-verion>
```

You can get the `<lastest-verion>` [here](https://dashboard.daocloud.io/packages/98ecf23a-8bd1-4135-a1c0-ac18b6d27ab1).

In CI enviroment, you can use `gradle app:assembleRelease` instead of `./gradlew app:assembleRelease` to speed up your build.
