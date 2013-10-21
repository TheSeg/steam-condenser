{% highlight ruby %}
id = SteamId.new 'demomenz'
stats = id.game_stats 'tf2'
achievements = stats.achievements
{% endhighlight %}