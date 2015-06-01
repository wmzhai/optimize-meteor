# 什么是性能

本教程的主要目的是学会构建快速高效的Meteor程序，我们需要专注于一件事 -- **性能**。这主要可以分为2类:

- 时间性能(Time-Based Performance)
- 资源性能(Resource-Based Performance)

## 时间性能 - 做更快的app

从这个角度衡量，主要考虑讲处理时间降到最低，我们可以以时间标准来衡量。


### Response Time

对于web程序，响应时间一般是加载一个页面的完整时间。我们的目的是快速的app，所以我们需要构建低响应时间的程序。在meteor里面，我们需要构建3种类型的响应时间:

1. Method Response Time
2. Publication (pub/sub) Response Time
3. Initial Load Time

![](https://cldup.com/xs_prw0FBF.png)

### Throughput（吞吐量）

我们时常也记录吞吐量，主要看一下给定的时间周期内接受多少个请求。如果吞吐量较大的话，请求就会被放到队列处理，从而导致等待时间。


## 资源性能 - 做更高效的app

资源损耗主要包括如下三方面，这些是构建高效app的关键
- CPU使用
- 内存使用
- 带宽使用

![](https://cldup.com/pxeZ3cOrA2.png)




