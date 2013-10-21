{% highlight ruby %}
master = MasterServer.new(*MasterServer::GOLDSRC_MASTER_SERVER)
servers = master.servers
server = GoldSrcServer.new(*servers[rand servers.size])
{% endhighlight %}