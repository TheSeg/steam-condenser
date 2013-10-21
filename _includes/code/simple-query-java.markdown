{% highlight java %}
GoldSrcServer server = new GoldSrcServer("192.168.0.114", 27016);
server.initialize();
System.out.println(server.getPlayers());
{% endhighlight %}