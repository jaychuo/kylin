---
layout: docs
title:  Update Coprocessor
categories: howto
permalink: /docs30/howto/howto_update_coprocessor.html
---

Kylin leverages HBase coprocessor to optimize query performance. After new versions released, the RPC protocol may get changed, so user need to redeploy coprocessor to HTable.

There's a CLI tool to update HBase Coprocessor:

{% highlight Groff markup %}
$KYLIN_HOME/bin/kylin.sh org.apache.kylin.storage.hbase.util.DeployCoprocessorCLI default all
{% endhighlight %}