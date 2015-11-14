# apache-tomcat-7-rpm

[![Build Status](https://travis-ci.org/robertdebock/apache-tomcat-7.el7.svg?branch=master)](https://travis-ci.org/robertdebock/apache-tomcat-7.el7)

This repository contains sources of [Apache Tomcat 7](http://tomcat.apache.org) RPM's for [CentOS 7](https://www.centos.org/), [Red Hat 7](http://www.redhat.com/) or [Fedora](https://getfedora.org/).

[Travis-CI](https://travis-ci.org/robertdebock/apache-tomcat-7.el7) is being used to build, test and publish the RPM.

The RPMs are available on [Amazon S3](https://s3-eu-west-1.amazonaws.com/apache-tomcat7.el7/). To use these packages, copy this text into /etc/yum.repos.d/robertdebock.repo:

    [rpm-repos-el7]
    name=RPM Repos EL7
    baseurl=https://s3-eu-west-1.amazonaws.com/apache-tomcat7.el7/
    enabled=1
    gpgcheck=0

Or simply run:

    wget https://s3-eu-west-1.amazonaws.com/rpm-repos-el7/rpm-repos-el7-1-1.el7.noarch.rpm

And run:

    yum install apache-tomcat

Or [have a look in the repository](http://apache-tomcat7.el7.s3-eu-west-1.amazonaws.com/index.html) and download the RPM's.
    
Optional extra packages are:
- apache-tomcat-manager
- apache-tomcat-ROOT
- apache-tomcat-docs
- apache-tomcat-examples
- apache-tomcat-host-manager
