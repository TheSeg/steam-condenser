{% highlight java %}
SourceServer server = new SourceServer("127.0.0.1");
try {
  server.rconAuth("passw0rd");
  System.out.println(server.rconExec("status");
}
catch(RCONNoAuthException e) {
  System.err.println("Could not authenticate with the game server.");
}
{% endhighlight %}