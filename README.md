# ars

提供3大组件:

AppServer: http服务器，grpc服务器，分布式JOB服务器，MQ消费端

RCServer: 服务总线，负载均衡，服务发现

SPServer:微服务提供发布
* 统一配置，统一服务节
* 路径通配, 以IP+端口 作为服务目录
* 单机支持多AppServer, RCServer, SPServer部署
* 服务自动更新，自动下载脚步或主程序
* 提供HttpServer,FileSyncServer,LoggerServer,MerticServer,StaticFileServer,RPCServer,ProxyServer
* 配置通过ZK获取，可单机运行，不依赖集群
* 通过配置开关，提供系统跟踪日志
