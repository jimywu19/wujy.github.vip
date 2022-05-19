---
title: "Istio"
date: 2022-05-19T09:01:39+08:00
draft: false
---

# 1、其他
- HPA 
- VPA 

# 2、Consul

# 3、Eureka 

# 4、Zipkin

# 5、微服务架构
- dubbo
- springCloud

# 6、Knative 
 serviceless 

# 7、Istio
与**Kubernetes紧密结合**的适用于云原生场景的**Service Mesh形态**的用于**服务治理**的开发平台。  
**服务治理**：连接、安全、策略执行、可观测性

- UDPA(Universal Data Plane API)  
数据平面标准----**实例间网络流量**
- SMI(Service Mesh Interface)  
制平面标准----负责生成和部署控制数据平面行为的相关配置

## 7.1、Pilot
配置数据
VirtualService   DestinationRule Gateway ServiceEntry
- gRPC
- xDS

## 7.2、Envoy
**Service Mesh**
 服务网格，专注于处理服务间通信的**基础设施**，云原生组成的复杂拓扑中**可靠的传递请求**  
**Envoy** 服务网格的数据面代理
 动态服务发现、负载均衡、TLS、HTTP/2、gRPC代理、等等的实现角色

## 7.3、Mixer
- telemetry 数据收集
- policy 策略执行，访问控制   对接配额、授权、黑白名单的控制后端

## 7.4、citadel
安全组件 证书、密钥
tls认证、访问授权、通道加密

## 7.5、galley
控制面 配置管理

## 7.6、sidecar-injector
自动注入sidecar

## 7.7proxy

