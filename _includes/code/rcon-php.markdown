{% highlight php startinline %}
$server = new SourceServer('127.0.0.1');
try {
  $server->rconAuth('passw0rd');
  echo $server->rconExec('status');
}
catch(RCONNoAuthException $e) {
  trigger_error('Could not authenticate with the game server.',
    E_USER_ERROR);
}
{% endhighlight %}
