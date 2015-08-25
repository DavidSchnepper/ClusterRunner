---
layout: docs
title: Installation
prev_section: home
next_section: _auto_
permalink: /docs/installation/
---

We've done our best to make installing ClusterRunner insanely fast and easy.  This should take less than a minute.

## Install self-contained package
Pick a set of instructions based on your operating system.

**OS X**

{% highlight bash %}
~ $ mkdir -p ~/.clusterrunner/dist && cd ~/.clusterrunner && curl -L https://cloud.box.com/shared/static/pqln47ur9ektad5hxq4a.tgz > clusterrunner.tgz && tar -zxvf clusterrunner.tgz -C ./dist && cp ./dist/conf/default_clusterrunner.conf clusterrunner.conf && chmod 600 clusterrunner.conf
{% endhighlight %}

**Linux**

{% highlight bash %}
~ $ mkdir -p ~/.clusterrunner/dist && cd ~/.clusterrunner && curl -L https://cloud.box.com/shared/static/2pl4pi6ykvrbb9d06t4m.tgz > clusterrunner.tgz && tar -zxvf clusterrunner.tgz -C ./dist && cp ./dist/conf/default_clusterrunner.conf clusterrunner.conf && chmod 600 clusterrunner.conf
{% endhighlight %}

**Windows**

{% highlight bash%}
C:\> @powershell -NoProfile -ExecutionPolicy Bypass -Command "iex ((new-object net.webclient).DownloadString('https://cloud.box.com/shared/static/snpz1xcan76rpy112rdu33xjrvdmkcnk.ps1'))"
{% endhighlight %}

## Bash Alias

We suggest you add an alias for the clusterrunner binary to your shell startup file in order to easily execute ClusterRunner.

{% highlight bash %}
# Add this line to your ~/.bash_profile:
~ $ alias clusterrunner='~/.clusterrunner/dist/clusterrunner'
{% endhighlight %}
