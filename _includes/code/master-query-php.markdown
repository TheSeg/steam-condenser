{% highlight php startinline %}
$master = new MasterServer(MasterServer::GOLDSRC_MASTER_SERVER);
$servers = $master->getServers();
$randomServer = $servers[array_rand($servers)];
$server = new GoldSrcServer($randomServer[0], $randomServer[1]));
{% endhighlight %}
