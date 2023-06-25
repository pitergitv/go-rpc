[中文](readme-ZH.md)|English

[![Security Status](https://www.murphysec.com/platform3/v31/badge/1666706410635550720.svg)](https://www.murphysec.com/console/report/1666706410597801984/1666706410635550720)
## About go-dandelion

The go-dandelion project aims to provide developers with a project framework that integrates various components, making it easy to build projects and improve development efficiency. It eliminates the need to spend time on integrating different components, allowing developers to focus on business development.

**Integration**
+ [rpcx](https://github.com/smallnest/rpcx)
+ [fasthttp](https://github.com/valyala/fasthttp)
+ [fasthttp-routing](https://github.com/qiangxue/fasthttp-routing)
+ [gorm](https://github.com/go-gorm/gorm)
+ [redigo](https://github.com/gomodule/redigo)
+ [go-swagger](https://github.com/go-swagger/go-swagger)
+ [cobra](https://github.com/spf13/cobra)
+ [viper](https://github.com/spf13/viper)
+ [opentracing-go](https://github.com/opentracing/opentracing-go)

**Features**
+ Quickly create RPC services and HTTP services.
+ Initialize MySQL, Redis, logger, and trace links quickly through configuration.
+ Integrated logging, distributed tracing, rate limiting, circuit breaking, service registration, service discovery, and other features.
+ Customizable middleware and plugins.

## go-dandelion-cli Usage

## 1. Installation
```
go get github.com/gly-hub/go-dandelion/go-dandelion-cli@latest
go install github.com/gly-hub/go-dandelion/go-dandelion-cli@latest
```

## 2. Create a Project
Create a local project directory and create the corresponding project based on the prompts.
```shell
# Create an application
go-dandelion-cli app -n go-admin-example
# Enter the application directory
cd go-admin-example
# Build the service
go-dandelion-cli build -n go-admin-example
Enter the type of service to create, enter a number (1 for rpc, 2 for http): 1
RPC service name: example-server
Initialize MySQL (y/n): y
Initialize Redis (y/n): y
Initialize logger (y/n): y
Initialize trace links (y/n): y
```

## 3. Run the Project
```shell
cd example-server
# Enter the service directory
go build -o example-server
# Run the service
./example-server server
```

## 🔥Contributors

<a href="https://github.com/gly-hub/go-dandelion/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=gly-hub/go-dandelion" />
</a>

## ⭐ Star the project
if you find it interesting!

## Open Source
[Apache License, Version 2.0](LICENSE.txt)
