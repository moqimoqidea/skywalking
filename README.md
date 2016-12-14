Sky Walking
==========

<img src="http://wu-sheng.github.io/sky-walking/images/skywalking.png" alt="Sky Walking logo" height="90px" align="right" />

SkyWalking: Large-Scale Distributed Systems Tracing Infrastructure, also known Distributed Tracer。

[![Build Status](https://travis-ci.org/wu-sheng/sky-walking.svg?branch=master)](https://travis-ci.org/wu-sheng/sky-walking)
![license](https://img.shields.io/aur/license/yaourt.svg)
[![codebeat badge](https://codebeat.co/badges/579e4dce-1dc7-4f32-a163-c164eafa1335)](https://codebeat.co/projects/github-com-wu-sheng-sky-walking)
[![Join the chat at https://gitter.im/sky-walking/Lobby](https://badges.gitter.im/sky-walking/Lobby.svg)](https://gitter.im/sky-walking/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![sky-walking-org](https://img.shields.io/badge/organization-sky--walking--ecosystem-brightgreen.svg)](https://github.com/skywalking-developer)

[![Release Version](https://img.shields.io/badge/sky--walking-1.0--release-brightgreen.svg)](https://github.com/wu-sheng/sky-walking/releases)
[![Dev Version](https://img.shields.io/badge/sky--walking-2.0--ontesting-yellow.svg)](https://github.com/wu-sheng/sky-walking)

# Abstract
* An open source Large-Scale Distributed Systems Tracing Infrastructure, also known a ditributed tracer.
* Based on [Google Dapper Paper: Dapper, a Large-Scale Distributed Systems Tracing Infrastructure](http://research.google.com/pubs/pub36356.html), [read Simplified Chinese Version](http://duanple.blog.163.com/blog/static/70971767201329113141336/)
* Support popular rpc frameworks, such as [dubbo](https://github.com/alibaba/dubbo), [dubbox](https://github.com/dangdangdotcom/dubbox), [motan](https://github.com/weibocom/motan) etc., trigger email-alert when application occurs unexpected exception。
* Easy to deploy, **even in product mode** (since 2.0) . No need of Hadoop, HBase, or Cassandra Cluster.
* Pure Java server implements. provide gRPC (since 2.0)  and HTTP (since 2.1) cross-platform spans collecting service.


# Supported components
### web container
* Tomcat 7
* Tomcat 8

[![Tomcat 7 Test Docker](https://img.shields.io/badge/test--scenario-tomcat--7.0.73-brightgreen.svg)](https://hub.docker.com/r/skywalking/docker-tomcat-scenario/tags/)  [![Tomcat 8 Test Docker](https://img.shields.io/badge/test--scenario-tomcat--8.0.39-brightgreen.svg)](https://hub.docker.com/r/skywalking/docker-tomcat-scenario/tags/)


### database

* mysql
* oracle
* h2
* easily extend to support sybase, sqlserver, jtds, db2, informix

[![MySQL Test Docker](https://img.shields.io/badge/test--scenario-mysql--5.7-brightgreen.svg)](https://hub.docker.com/r/skywalking/docker-mysql-scenario/tags/)  <br/>
[![Oracle Test Docker](https://img.shields.io/badge/test--scenario-oracle--12.1.0.2-brightgreen.svg)](https://hub.docker.com/r/skywalking/docker-oracle-scenario/tags/)  <br/>
[![H2 Test Docker](https://img.shields.io/badge/test--scenario-h2--1.3.176-brightgreen.svg)](https://hub.docker.com/r/skywalking/docker-h2-scenario/tags/)


### rpc framework
* dubbo 
* dubbox 
* httpClient
* motan

[![Dubbo Test Docker](https://img.shields.io/badge/test--scenario-dubbo--2.5.3-brightgreen.svg)](https://hub.docker.com/r/skywalking/docker-dubbo-scenario/tags/)  <br/>
[![Dubbox Test Docker](https://img.shields.io/badge/test--scenario-dubbox--2.8.4.rpc-brightgreen.svg)](https://hub.docker.com/r/skywalking/docker-dubbox-scenario/tags/)  [![Dubbox Test Docker](https://img.shields.io/badge/test--scenario-dubbox--2.8.4.rest-brightgreen.svg)](https://hub.docker.com/r/skywalking/docker-dubbox-scenario/tags/)  <br/>
[![HttpClient Test Docker](https://img.shields.io/badge/test--scenario-httpclient--4.2-brightgreen.svg)](https://hub.docker.com/r/skywalking/docker-httpclient-scenario/tags/)  [![HttpClient Test Docker](https://img.shields.io/badge/test--scenario-httpclient--4.3-brightgreen.svg)](https://hub.docker.com/r/skywalking/docker-httpclient-scenario/tags/)  <br/>
[![Motan Test Docker](https://img.shields.io/badge/test--scenario-motan--0.2.1-brightgreen.svg)](https://hub.docker.com/r/skywalking/docker-motan-scenario/tags/)

### cache
* jedis

[![Jedis Test Docker](https://img.shields.io/badge/test--scenario-jedis--2.8.1-brightgreen.svg)](https://hub.docker.com/r/skywalking/docker-jedis-scenario/tags/)  

_All test scenarios base on Docker Tech._

# Contributors
* 吴晟 [wusheng](https://github.com/wu-sheng) &nbsp;&nbsp;wu.sheng@foxmail.com
* 张鑫 [zhangxin](https://github.com/ascrutae) &nbsp;&nbsp;


_Chinese Articles about sky-walking and distributed tracer_

<img src="http://wu-sheng.github.io/sky-walking/sample-code/screenshoot/chatapp/toutiao.JPG" alt="Sky Walking TouTiao" height="280px" />

___

<a href="https://github.com/wu-sheng/sky-walking">
<img src="http://wu-sheng.github.io/sky-walking/sample-code/award/oneapm-award.png" alt="OneAPM Open Source Achievement Award" height="110px" align="left" />
</a>

In October 2016, Sky Walking won `OneAPM Open Source Achievement Award`. The award appreciates sky walking for its "*contribution to popularization of APM technology*". <br/>
[OneAPM](http://www.oneapm.com/) will provide financial support for the project in 2016-2017.<br/><br/> 
Thanks all users of sky walking project.
___


# Quick View
* distributed tracer
![追踪连路图1](http://wu-sheng.github.io/sky-walking/sample-code/screenshoot/1.0b/callChain.png)

![追踪连路图2](http://wu-sheng.github.io/sky-walking/sample-code/screenshoot/1.0b/callChainDetail.png)

![追踪连路图3](http://wu-sheng.github.io/sky-walking/sample-code/screenshoot/1.0b/callChainLog.png)

* alarm mail
![告警邮件](http://wu-sheng.github.io/sky-walking/sample-code/screenshoot/1.0b/alarmMail.png)

# Document
* [WIKI](https://github.com/wu-sheng/sky-walking/wiki)
