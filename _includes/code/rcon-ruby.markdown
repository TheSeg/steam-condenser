{% highlight ruby %}
server = SourceServer.new('127.0.0.1')
begin
  server.rcon_auth('passw0rd')
  puts server.rcon_exec('status')
rescue RCONNoAuthException
  warn 'Could not authenticate with the game server.'
end
{% endhighlight %}