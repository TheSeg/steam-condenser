{% highlight php startinline %}
$server = new GoldSrcServer('192.168.0.114', 27016);
$server->initialize();
echo $server->getPlayers();
{% endhighlight %}
