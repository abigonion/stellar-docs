---
title: 硬件需求
---

# 注意事项

 Stellar 网络是一个持续增长的系统，硬件需求会随着网络的增长而增长。因此在选用配置时，请务必考虑到这一点。

如果您选择使用下面列出的最低配置要求，您可能会在网络流量高峰期间遇到一些延迟，因为您的节点需要花费一些时间来同步最新的网络数据。为了获得流畅的体验，我们推荐您优先选用推荐配置。

随着我们对代码库的进一步改进，我们将尽最大努力使这个文档保持最新。

# 节点

## Stellar-Core

Stellar-Core 实例是 Stellar 网络节点的一部分，因此需要足够大的硬盘来支撑这不断增长的网络。

### 最低配置
**CPU**: 4-Core (8-Thread) Intel i7/Xeon 或同等产品 (AWS 上的 c5.xlarge 机型)\
**RAM**: 8GB DDR4\
**SSD**: 64GB

### 推荐配置
**CPU**: 8-Core (16-Thread) Intel i7/Xeon 或同等产品 (AWS 上的 c5.2xlarge 机型)\
**RAM**: 16GB DDR4\
**SSD**: 120GB

## Horizon

Horizon 实例会从网络中提取数据，因此需要足够大硬盘来保存从网络中提取的事务数据。

Horizon 会对它的数据库进行大量的操作，而以下配置并没有将运行此数据库的需要消耗资源计算在内。所以您需要将数据库允许在另一台独立的服务器上，或者适当提高机器的配置。

### 最低配置
**CPU**: 8-Core (16-Thread) Intel i7/Xeon 或同等产品 (AWS 上的 c5.2xlarge 机型)\
**RAM**: 16GB DDR4\
**SSD**: 64GB

### 推荐配置
**CPU**: 16-Core (32-Thread) Intel i7/Xeon 或同等产品 (AWS 上的 c5.4xlarge 机型)\
**RAM**: 32GB DDR4\
**SSD**: 120GB

# 锚点需要的服务

这些锚点服务的硬件要求取决于您自己的内部使用情况，也就是说这些硬件要求不会随着 Stellar 网络容量的增加而增加。我们建议您将每项服务运行在一台独立的服务器上，但如果您愿意的话，也可以使用 VM 技术将多个服务运行在单个服务器上。

## 桥接服务器

### 最低配置
**CPU**: 2-Core (4-Thread) Intel i7/Xeon or 或同等产品 (AWS 上的 c5.large 机型)\
**RAM**: 4GB DDR3/DDR4\
**SSD**: 需要一个数据库来保存已处理的事务。上述的 CPU 和 RAM 要求并没有将运行此数据库的需要消耗资源计算在内。数据库的大小取决于您对网络的使用情况。在最开始，您可以配置一个 20GB 的磁盘。

### 推荐配置
**CPU**: 4-Core (8-Thread) Intel i7/Xeon or 或同等产品 (AWS 上的 c5.xlarge 机型)\
**RAM**: 8GB DDR4\
**SSD**: 需要一个数据库来保存已处理的事务。上述的 CPU 和 RAM 要求并没有将运行此数据库的需要消耗资源计算在内。数据库的大小取决于您对网络的使用情况。在最开始，您可以配置一个 20GB 的磁盘。

## 联邦服务器

### 最低配置
**CPU**: 2-Core (4-Thread) Intel i7/Xeon 或同等产品 (AWS 上的 c5.large 机型)\
**RAM**: 4GB DDR3/DDR4\
**SSD**: 需要一个数据库来保存联邦记录表。上述的 CPU 和 RAM 要求并没有将运行此数据库的需要消耗资源计算在内。数据库的大小取决于您保存了多少账户。请参阅日志获取更多信息。

### 推荐配置
**CPU**: 4-Core (8-Thread) Intel i7/Xeon 或同等产品 (AWS 上的 c5.xlarge 机型)\
**RAM**: 8GB DDR4\
**SSD**: 需要一个数据库来保存联邦记录表。上述的 CPU 和 RAM 要求并没有将运行此数据库的需要消耗资源计算在内。数据库的大小取决于您保存了多少账户。请参阅日志获取更多信息。

## 合规服务器

### 最低配置
**CPU**: 2-Core (4-Thread) Intel i7/Xeon 或同等产品 (AWS 上的 c5.large 机型)\
**RAM**: 4GB DDR3/DDR4\
**SSD**: 需要一个数据库来保存已处理的事务。上述的 CPU 和 RAM 要求并没有将运行此数据库的需要消耗资源计算在内。数据库的大小取决于您对网络的使用情况。在最开始时，您可以配置一个 20GB 的磁盘。

### 推荐配置
**CPU**: 4-Core (8-Thread) Intel i7/Xeon 或同等产品 (AWS 上的 c5.xlarge 机型)\
**RAM**: 8GB DDR4\
**SSD**: 需要一个数据库来保存已处理的事务。上述的 CPU 和 RAM 要求并没有将运行此数据库的需要消耗资源计算在内。数据库的大小取决于您对网络的使用情况。在最开始时，您可以配置一个 20GB 的磁盘。