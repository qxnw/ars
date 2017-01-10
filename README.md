#ARS
基于ZK提供集群的可单机运行的基础服务及功能，提供的功能包括:
* 微服务化，基于LUA脚本，提供grpc，http等服务
* 服务自动上线及发现，根据ZK任务配置启动服务，自动上线，消费端自动发现服务
* 负载均衡 提供基于轮循，响应速度，服务端负载等机制
* 提供多种服务支持 http服务器，反向代理服务，grpc服务器，分布式JOB服务器，自动JOB， MQ消费端
* 其它组件支持 oracle，memcache，redis，influxdb，es，stomp，metric，logger，kafka

# ARS包含三大基础服务器（AppServer, RCServer, SPServer）

#AppServer（应用服务）
系统的业务逻辑服务，外部的服务（http server，rpc server，proxy server）或内部服务（mq consumer，job）
#RCServer
系统负载均衡器，服务发现（sp server），跨域访问，服务总线
#SPServer
系统基础服务提供及发布，通过ZK发布服务，接受由负载中心发起的RPC调用
