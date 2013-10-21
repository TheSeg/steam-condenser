{% highlight php startinline %}
$id = SteamId::create('demomenz');
$stats = $id->getGameStats('tf2');
$achievements = $stats->getAchievements();
{% endhighlight %}
